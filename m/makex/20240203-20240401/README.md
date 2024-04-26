# Comparing `tmp/makex-20240203.tar.gz` & `tmp/makex-20240401.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makex-20240203.tar", last modified: Sun Feb 11 03:41:58 2024, max compression
+gzip compressed data, was "makex-20240401.tar", last modified: Fri Apr 26 20:00:55 2024, max compression
```

## Comparing `makex-20240203.tar` & `makex-20240401.tar`

### file list

```diff
@@ -1,57 +1,64 @@
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-02-11 03:41:58.990490 makex-20240203/
--rw-r--r--   0 nate      (1000) nate      (1000)     2225 2024-02-11 03:41:58.990490 makex-20240203/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)     1638 2024-02-11 03:41:55.000000 makex-20240203/README.md
--rw-rw-r--   0 nate      (1000) nate      (1000)     1495 2024-02-11 03:41:55.000000 makex-20240203/pyproject.toml
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-02-11 03:41:58.986490 makex-20240203/python/
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-02-11 03:41:58.988490 makex-20240203/python/makex/
--rw-rw-r--   0 nate      (1000) nate      (1000)    40551 2024-02-11 03:41:55.000000 makex-20240203/python/makex/__main__.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     2529 2024-02-11 03:41:55.000000 makex-20240203/python/makex/_logging.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     5944 2024-02-11 03:41:55.000000 makex-20240203/python/makex/_shtab.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      697 2024-02-11 03:41:55.000000 makex-20240203/python/makex/api.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    15755 2024-02-11 03:41:55.000000 makex-20240203/python/makex/build_path.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      721 2024-02-11 03:41:55.000000 makex-20240203/python/makex/colors.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     8847 2024-02-11 03:41:55.000000 makex-20240203/python/makex/configuration.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     4199 2024-02-11 03:41:55.000000 makex-20240203/python/makex/constants.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     6547 2024-02-11 03:41:55.000000 makex-20240203/python/makex/context.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-02-11 03:41:58.986490 makex-20240203/python/makex/data/
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-02-11 03:41:58.989490 makex-20240203/python/makex/data/completions/
--rw-rw-r--   0 nate      (1000) nate      (1000)     9106 2024-02-11 03:41:55.000000 makex-20240203/python/makex/data/completions/makex.bash
--rw-rw-r--   0 nate      (1000) nate      (1000)     5599 2024-02-11 03:41:55.000000 makex-20240203/python/makex/data/completions/makex.zsh
--rw-rw-r--   0 nate      (1000) nate      (1000)     2410 2024-02-11 03:41:55.000000 makex-20240203/python/makex/errors.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    47419 2024-02-11 03:41:55.000000 makex-20240203/python/makex/executor.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     7116 2024-02-11 03:41:55.000000 makex-20240203/python/makex/executor_test.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    11466 2024-02-11 03:41:55.000000 makex-20240203/python/makex/file_checksum.py
--rw-rw-r--   0 nate      (1000) nate      (1000)        0 2024-02-11 03:41:55.000000 makex-20240203/python/makex/file_checksum_test.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     3637 2024-02-11 03:41:55.000000 makex-20240203/python/makex/file_system.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     3452 2024-02-11 03:41:55.000000 makex-20240203/python/makex/flags.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    96848 2024-02-11 03:41:55.000000 makex-20240203/python/makex/make_file.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     4736 2024-02-11 03:41:55.000000 makex-20240203/python/makex/makefile_test.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     5571 2024-02-11 03:41:55.000000 makex-20240203/python/makex/metadata.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     2879 2024-02-11 03:41:55.000000 makex-20240203/python/makex/metadata_file.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     4912 2024-02-11 03:41:55.000000 makex-20240203/python/makex/metadata_sqlite.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      455 2024-02-11 03:41:55.000000 makex-20240203/python/makex/metadata_sqlite_test.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      562 2024-02-11 03:41:55.000000 makex-20240203/python/makex/metadata_test.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     3157 2024-02-11 03:41:55.000000 makex-20240203/python/makex/patterns.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      600 2024-02-11 03:41:55.000000 makex-20240203/python/makex/patterns_test.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-02-11 03:41:58.989490 makex-20240203/python/makex/platform_object/
--rw-rw-r--   0 nate      (1000) nate      (1000)       43 2024-02-11 03:41:55.000000 makex-20240203/python/makex/platform_object/__init__.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     4691 2024-02-11 03:41:55.000000 makex-20240203/python/makex/platform_object/platform_object.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      342 2024-02-11 03:41:55.000000 makex-20240203/python/makex/platform_object/platform_test.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     2216 2024-02-11 03:41:55.000000 makex-20240203/python/makex/protocols.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    18354 2024-02-11 03:41:55.000000 makex-20240203/python/makex/python_script.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     6196 2024-02-11 03:41:55.000000 makex-20240203/python/makex/reflink.py
--rw-rw-r--   0 nate      (1000) nate      (1000)      217 2024-02-11 03:41:55.000000 makex-20240203/python/makex/reflink_test.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     3952 2024-02-11 03:41:55.000000 makex-20240203/python/makex/run.py
--rw-rw-r--   0 nate      (1000) nate      (1000)    13159 2024-02-11 03:41:55.000000 makex-20240203/python/makex/target.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     3931 2024-02-11 03:41:55.000000 makex-20240203/python/makex/ui.py
--rw-rw-r--   0 nate      (1000) nate      (1000)       19 2024-02-11 03:41:55.000000 makex-20240203/python/makex/version.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     9652 2024-02-11 03:41:55.000000 makex-20240203/python/makex/workspace.py
--rw-rw-r--   0 nate      (1000) nate      (1000)     1054 2024-02-11 03:41:55.000000 makex-20240203/python/makex/workspace_test.py
-drwxrwxr-x   0 nate      (1000) nate      (1000)        0 2024-02-11 03:41:58.989490 makex-20240203/python/makex.egg-info/
--rw-r--r--   0 nate      (1000) nate      (1000)     2225 2024-02-11 03:41:58.000000 makex-20240203/python/makex.egg-info/PKG-INFO
--rw-rw-r--   0 nate      (1000) nate      (1000)     1391 2024-02-11 03:41:58.000000 makex-20240203/python/makex.egg-info/SOURCES.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)        1 2024-02-11 03:41:58.000000 makex-20240203/python/makex.egg-info/dependency_links.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       46 2024-02-11 03:41:58.000000 makex-20240203/python/makex.egg-info/entry_points.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)      150 2024-02-11 03:41:58.000000 makex-20240203/python/makex.egg-info/requires.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)        6 2024-02-11 03:41:58.000000 makex-20240203/python/makex.egg-info/top_level.txt
--rw-rw-r--   0 nate      (1000) nate      (1000)       38 2024-02-11 03:41:58.990490 makex-20240203/setup.cfg
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.538812 makex-20240401/
+-rw-r--r--   0 nate      (1000) nate      (1000)     3232 2024-04-26 20:00:55.537812 makex-20240401/PKG-INFO
+-rw-r--r--   0 nate      (1000) nate      (1000)     1912 2024-04-26 20:00:53.000000 makex-20240401/README.md
+-rw-r--r--   0 nate      (1000) nate      (1000)     2126 2024-04-26 20:00:53.000000 makex-20240401/pyproject.toml
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.530812 makex-20240401/python/
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.531812 makex-20240401/python/benchmarks/
+-rw-r--r--   0 nate      (1000) nate      (1000)     1518 2024-04-26 20:00:53.000000 makex-20240401/python/benchmarks/hashing_benchmark_test.py
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.535812 makex-20240401/python/makex/
+-rw-r--r--   0 nate      (1000) nate      (1000)    43219 2024-04-26 20:00:53.000000 makex-20240401/python/makex/__main__.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     2126 2024-04-26 20:00:53.000000 makex-20240401/python/makex/_logging.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     6016 2024-04-26 20:00:53.000000 makex-20240401/python/makex/_shtab.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)      693 2024-04-26 20:00:53.000000 makex-20240401/python/makex/api.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    15755 2024-04-26 20:00:53.000000 makex-20240401/python/makex/build_path.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      945 2024-04-26 20:00:53.000000 makex-20240401/python/makex/colors.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     9448 2024-04-26 20:00:53.000000 makex-20240401/python/makex/configuration.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     4919 2024-04-26 20:00:53.000000 makex-20240401/python/makex/constants.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     6558 2024-04-26 20:00:53.000000 makex-20240401/python/makex/context.py
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.530812 makex-20240401/python/makex/data/
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.536811 makex-20240401/python/makex/data/completions/
+-rw-r--r--   0 nate      (1000) nate      (1000)     9618 2024-04-26 20:00:53.000000 makex-20240401/python/makex/data/completions/makex.bash
+-rw-r--r--   0 nate      (1000) nate      (1000)     6146 2024-04-26 20:00:53.000000 makex-20240401/python/makex/data/completions/makex.zsh
+-rw-rw-r--   0 nate      (1000) nate      (1000)     2411 2024-04-26 20:00:53.000000 makex-20240401/python/makex/errors.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    50541 2024-04-26 20:00:53.000000 makex-20240401/python/makex/executor.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     7517 2024-04-26 20:00:53.000000 makex-20240401/python/makex/executor_test.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    11770 2024-04-26 20:00:53.000000 makex-20240401/python/makex/file_checksum.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:53.000000 makex-20240401/python/makex/file_checksum_test.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     6332 2024-04-26 20:00:53.000000 makex-20240401/python/makex/file_cloning.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      228 2024-04-26 20:00:53.000000 makex-20240401/python/makex/file_cloning_test.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     3656 2024-04-26 20:00:53.000000 makex-20240401/python/makex/file_system.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     3806 2024-04-26 20:00:53.000000 makex-20240401/python/makex/flags.py
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.536811 makex-20240401/python/makex/integrations/
+-rw-r--r--   0 nate      (1000) nate      (1000)      774 2024-04-26 20:00:53.000000 makex-20240401/python/makex/integrations/intellij.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      484 2024-04-26 20:00:53.000000 makex-20240401/python/makex/integrations/vscode.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    83180 2024-04-26 20:00:53.000000 makex-20240401/python/makex/makex_file.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    36614 2024-04-26 20:00:53.000000 makex-20240401/python/makex/makex_file_parser.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     6970 2024-04-26 20:00:53.000000 makex-20240401/python/makex/makex_file_parser_test.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    11283 2024-04-26 20:00:53.000000 makex-20240401/python/makex/makex_file_types.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     5654 2024-04-26 20:00:53.000000 makex-20240401/python/makex/metadata.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     2879 2024-04-26 20:00:53.000000 makex-20240401/python/makex/metadata_file.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     5519 2024-04-26 20:00:53.000000 makex-20240401/python/makex/metadata_sqlite.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      487 2024-04-26 20:00:53.000000 makex-20240401/python/makex/metadata_sqlite_test.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      671 2024-04-26 20:00:53.000000 makex-20240401/python/makex/metadata_test.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     3157 2024-04-26 20:00:53.000000 makex-20240401/python/makex/patterns.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)      600 2024-04-26 20:00:53.000000 makex-20240401/python/makex/patterns_test.py
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.536811 makex-20240401/python/makex/platform_object/
+-rw-rw-r--   0 nate      (1000) nate      (1000)       43 2024-04-26 20:00:53.000000 makex-20240401/python/makex/platform_object/__init__.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     4960 2024-04-26 20:00:53.000000 makex-20240401/python/makex/platform_object/platform_object.py
+-rw-r--r--   0 nate      (1000) nate      (1000)      484 2024-04-26 20:00:53.000000 makex-20240401/python/makex/platform_object/platform_test.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     2216 2024-04-26 20:00:53.000000 makex-20240401/python/makex/protocols.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    25641 2024-04-26 20:00:53.000000 makex-20240401/python/makex/python_script.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     3962 2024-04-26 20:00:53.000000 makex-20240401/python/makex/run.py
+-rw-r--r--   0 nate      (1000) nate      (1000)    13762 2024-04-26 20:00:53.000000 makex-20240401/python/makex/target.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     4109 2024-04-26 20:00:53.000000 makex-20240401/python/makex/ui.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)       19 2024-04-26 20:00:53.000000 makex-20240401/python/makex/version.py
+-rw-r--r--   0 nate      (1000) nate      (1000)     9577 2024-04-26 20:00:53.000000 makex-20240401/python/makex/workspace.py
+-rw-rw-r--   0 nate      (1000) nate      (1000)     1054 2024-04-26 20:00:53.000000 makex-20240401/python/makex/workspace_test.py
+drwxr-xr-x   0 nate      (1000) nate      (1000)        0 2024-04-26 20:00:55.536811 makex-20240401/python/makex.egg-info/
+-rw-r--r--   0 nate      (1000) nate      (1000)     3232 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/PKG-INFO
+-rw-r--r--   0 nate      (1000) nate      (1000)     1596 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/SOURCES.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)        1 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/dependency_links.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)       71 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/entry_points.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)      210 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/requires.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)       17 2024-04-26 20:00:55.000000 makex-20240401/python/makex.egg-info/top_level.txt
+-rw-r--r--   0 nate      (1000) nate      (1000)       38 2024-04-26 20:00:55.538812 makex-20240401/setup.cfg
```

### Comparing `makex-20240203/PKG-INFO` & `makex-20240401/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,61 @@
 Metadata-Version: 2.1
 Name: makex
-Version: 20240203
+Version: 20240401
 Summary: Build tool
 Author: Nate Skulic, MetaCompany
+Keywords: build,make,automation
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: toml>=0.10.2
 Requires-Dist: progressbar2>=4.3.2
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Requires-Dist: shtab; extra == "build"
+Requires-Dist: pex; extra == "build"
+Requires-Dist: nuitka; extra == "build"
+Requires-Dist: pytest; extra == "build"
+Requires-Dist: shtab; extra == "build"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov~=3.0.0; extra == "test"
 Provides-Extra: documents
 Requires-Dist: sphinx; extra == "documents"
 Requires-Dist: sphinx-better-theme; extra == "documents"
+Requires-Dist: sphinx-notfound-page; extra == "documents"
 Requires-Dist: myst-parser; extra == "documents"
 Requires-Dist: markdown-it-py[linkify,plugins]; extra == "documents"
 
 # makex
 
 <!-- heading -->
 
-Makex is a new and simplified automation tool, similar to the original [Make](https://en.wikipedia.org/wiki/Make_(software)).
+Makex is a new and simplified build and automation tool, similar to the original [Make](https://en.wikipedia.org/wiki/Make_(software)).
 
 It __*makex*__ stuff happen. 🙂
 
 <!-- features -->
 
+
+## What Makex is used for
+
+- Compiling software/applications/firmware
+- Building filesystems/trees/file archives
+- Building and deploying websites and web applications
+- Running things in a repeatable manner
+- Replacing most or all of the other build systems
+
 ## Features
 
 - Familiar Syntax
 - File Hashing and Checksums
 - Dependency Graphs
 - Caching
 - Workspaces
@@ -45,46 +71,46 @@
 - Support: [Google Groups](http://groups.google.com/group/makex) or [makex@googlegroups.com](mailto://makex@googlegroups.com)
 
 <!-- quick-start -->
 
 
 ## Quick Start
 
-- Install:
+1. Install:
 
   ```shell
   pip install makex
   ```
 
-- Define a Makex file (name it `Makexfile`):
+2. Define a Makex file (name it `Makexfile`):
 
   ```python
   #!makex
   
-  target(
+  task(
       name="hello-world",
-      runs=[
+      steps=[
           write("hello-world.txt", "Hello World!"),
   
           # or, you can use the shell, but it's not recommended:
           # shell(f"echo 'Hello World!' > {path('hello-world')}/hello-world.txt"),
       ],
       outputs=[
           "hello-world.txt",
       ],
   )
   ```
 
-- Run makex and the target:
+3. Run makex and the target:
 
   ```shell
   makex run :hello-world
   ```
  
-- A file at `_output_/hello-world/hello-world.txt` will have the following contents:
+4. A file at `_output_/hello-world/hello-world.txt` will have the following contents:
 
   ```
   Hello World!
   ```
 
 
 ## Limitations
```

### Comparing `makex-20240203/README.md` & `makex-20240401/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 # makex
 
 <!-- heading -->
 
-Makex is a new and simplified automation tool, similar to the original [Make](https://en.wikipedia.org/wiki/Make_(software)).
+Makex is a new and simplified build and automation tool, similar to the original [Make](https://en.wikipedia.org/wiki/Make_(software)).
 
 It __*makex*__ stuff happen. 🙂
 
 <!-- features -->
 
+
+## What Makex is used for
+
+- Compiling software/applications/firmware
+- Building filesystems/trees/file archives
+- Building and deploying websites and web applications
+- Running things in a repeatable manner
+- Replacing most or all of the other build systems
+
 ## Features
 
 - Familiar Syntax
 - File Hashing and Checksums
 - Dependency Graphs
 - Caching
 - Workspaces
@@ -27,46 +36,46 @@
 - Support: [Google Groups](http://groups.google.com/group/makex) or [makex@googlegroups.com](mailto://makex@googlegroups.com)
 
 <!-- quick-start -->
 
 
 ## Quick Start
 
-- Install:
+1. Install:
 
   ```shell
   pip install makex
   ```
 
-- Define a Makex file (name it `Makexfile`):
+2. Define a Makex file (name it `Makexfile`):
 
   ```python
   #!makex
   
-  target(
+  task(
       name="hello-world",
-      runs=[
+      steps=[
           write("hello-world.txt", "Hello World!"),
   
           # or, you can use the shell, but it's not recommended:
           # shell(f"echo 'Hello World!' > {path('hello-world')}/hello-world.txt"),
       ],
       outputs=[
           "hello-world.txt",
       ],
   )
   ```
 
-- Run makex and the target:
+3. Run makex and the target:
 
   ```shell
   makex run :hello-world
   ```
  
-- A file at `_output_/hello-world/hello-world.txt` will have the following contents:
+4. A file at `_output_/hello-world/hello-world.txt` will have the following contents:
 
   ```
   Hello World!
   ```
 
 
 ## Limitations
```

### Comparing `makex-20240203/pyproject.toml` & `makex-20240401/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -17,49 +17,71 @@
     "toml>=0.10.2",
     "progressbar2>=4.3.2",
 ]
 authors = [
     {name = "Nate Skulic"},
     {name = "MetaCompany" },
 ]
+keywords = ["build", "make", "automation"]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    #"License :: OSI Approved :: Apache Software License",
+    "Operating System :: Unix",
+    "Operating System :: POSIX :: Linux",
+   # "Operating System :: MacOS :: MacOS X",
+    "Programming Language :: Python",
+    "Programming Language :: Python :: Implementation :: CPython",
+    "Topic :: Software Development :: Build Tools",
+    "Topic :: Utilities",
+]
+
 
 [tool.setuptools.dynamic]
 version = { attr = "makex.version.VERSION" }
 
 [project.optional-dependencies]
+build = [
+    "build",
+    "shtab",
+    "pex",
+    "nuitka",
+    "pytest",
+    "shtab",
+]
 test = [
     "pytest",
     "pytest-cov ~=3.0.0",
 ]
 documents = [
     "sphinx",
     "sphinx-better-theme",
+    "sphinx-notfound-page",
     "myst-parser",
     "markdown-it-py[linkify,plugins]"
 ]
 
 [project.scripts]
 makex = "makex.__main__:main"
-
+mx = "makex.__main__:main"
 
 [tool.setuptools.packages.find]
 where = ["python"]
-#include = ["*", "themes"]
 namespaces = true
 
 [tool.setuptools.package-data]
 "makex.data.completions" =[
     "*.bash",
     "*.zsh",
 ]
-#"documents" = ["documents"]
 
 [tool.pytest.ini_options]
 log_cli = true
 log_cli_level = "5"
 log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
 log_cli_date_format = "%Y-%m-%d %H:%M:%S"
 addopts = [
     "--import-mode=importlib",
 ]
 pythonpath = "."
+cache_dir = "~/.cache/pytest"
```

### Comparing `makex-20240203/python/makex/__main__.py` & `makex-20240401/python/makex/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,56 +20,62 @@
     Any,
     Literal,
     Optional,
     Sequence,
     Union,
 )
 
-from makex._logging import initialize_logging
+from makex._logging import (
+    initialize_logging,
+    trace,
+)
 from makex.build_path import get_build_path
 from makex.colors import (
     Colors,
     ColorsNames,
     NoColors,
 )
 from makex.configuration import (
+    ConfigurationError,
     collect_configurations,
     evaluate_configuration_environment,
     read_configuration,
 )
 from makex.constants import (
     CONFIGURATION_ARGUMENT_ENABLED,
+    DIRECT_REFERENCES_TO_MAKEX_FILES,
     WORKSPACE_ARGUMENT_ENABLED,
 )
 from makex.context import Context
 from makex.errors import (
     CacheError,
+    Error,
     ExecutionError,
     GenericSyntaxError,
 )
 from makex.executor import Executor
 from makex.flags import VARIANTS_ENABLED
-from makex.make_file import (
-    MakexFileCycleError,
-    ResolvedTargetReference,
+from makex.makex_file import MakexFileCycleError
+from makex.makex_file_parser import (
     TargetGraph,
     parse_makefile_into_graph,
 )
+from makex.makex_file_types import ResolvedTargetReference
 from makex.python_script import (
     PythonScriptError,
     PythonScriptFileError,
 )
 from makex.run import (
     get_running_process_ids,
     run,
 )
 from makex.target import EvaluatedTargetGraph
 from makex.ui import (
     UI,
-    isansitty,
+    is_ansi_tty,
     pretty_makex_file_exception,
 )
 from makex.version import VERSION
 from makex.workspace import (
     current_workspace,
     get_workspace,
     which_workspace,
@@ -102,15 +108,15 @@
     path: Path
     type: ScopePart = None
 
 
 def is_color_enabled(color_argument: Literal["no", "auto", "off", "on", "yes"]):
     color_argument = color_argument.lower()
     if color_argument == "auto":
-        return isansitty()
+        return is_ansi_tty()
     elif color_argument in {"no", "off"}:
         return False
     elif color_argument in {"yes", "on"}:
         return True
 
     return None
 
@@ -259,15 +265,15 @@
             type=int,
             help="Worker threads to spawn for running/evaluating targets in parallel. Automatically detected.",
             default=cpus
         )
 
     parser = ArgumentParser(
         prog="makex",
-        description="""Makex command line program.""",
+        description="""Makex command line program.\n\nSee https://meta.company/go/makex for the latest documentation.""",
         epilog="""""", #parents=[base_parser],
     )
     _add_global_arguments(parser, cache, documentation)
 
     base_parser = ArgumentParser(add_help=False)
     _add_global_arguments(base_parser, cache, documentation, help=SUPPRESS)
 
@@ -282,32 +288,34 @@
         help="Commands you may enter.",
         required=True,
     )
 
     ######### run
     subparser = subparsers.add_parser(
         "run",
-        help="Run a target or list of targets.",
-        description="Run a target or list of targets.",
+        help="Run a task or list of tasks.",
+        description="Run a task or list of tasks.",
         parents=[base_parser],
     )
+    subparser.set_defaults(command_function=main_run)
+
     action = subparser.add_argument(
-        "targets",
+        "tasks",
         nargs="+",
     )
     action.complete = COMPLETE_TARGET
     subparser.add_argument(
         "--directory",
-        help="Change to directory before evaluating targets.",
+        help="Change to directory before evaluating tasks.",
     ) #"-C",
 
     subparser.add_argument(
         "--force",
         action="store_true",
-        help="Always run all targets even if they don't need to be.",
+        help="Always run all task even if they don't need to be.",
     ) #"-f",
 
     subparser.add_argument(
         "--dry",
         action="store_true",
         default=False,
         help="Do a dry run. Nothing will be executed.",
@@ -332,34 +340,33 @@
     if True:
         # XXX: Currently disabled.
         add_threads_argument(subparser)
 
     ######## path
     subparser = subparsers.add_parser(
         "path",
-        help="Get the output path of a target.",
-        description="Get the output path of a target.",
+        help="Get the output path of a task.",
+        description="Get the output path of a task.",
         parents=[base_parser],
     )
     subparser.add_argument(
-        "target",
-        help="Name and optional path of a target. //path:name, //:name, :name are all valid."
+        "task", help="Name and optional path of a task. //path:name, //:name, :name are all valid."
     )
-    # XXX: enable this whenw e
     subparser.add_argument(
         "--real",
         action="store_true",
         help="Return cache path. This may be slower as it must resolve Workspaces.",
         default=False,
     ) #"-r",
+    subparser.set_defaults(command_function=main_get_path)
 
     ######## dot
     subparser = subparsers.add_parser(
         "dot",
-        help="Create a dot depedency graph of targets. Printed to standard output.",
+        help="Create a dot dependency graph of tasks. Printed to standard output.",
         parents=[base_parser],
     )
     subparser.add_argument("targets", nargs="+")
     subparser.add_argument(
         "--files",
         help="Include/evaluate files/globs. May be slow.",
     ) # "-f", "-f",
@@ -372,48 +379,53 @@
         help="Specify file ignore patterns for input/output files.",
     )
     add_threads_argument(subparser)
 
     ######## affected
     subparser = subparsers.add_parser(
         "affected",
-        help="Return a list of targets affected by changes to the specified files.",
+        help="Return a list of tasks affected by changes to the specified files.",
         parents=[base_parser],
     )
+    subparser.set_defaults(command_function=main_affected)
     subparser.add_argument("files", nargs="+")
+
     add_threads_argument(subparser)
 
     ######## inputs
     subparser = subparsers.add_parser(
         "inputs",
-        help="Return the input files of a target. Evaluates the file.",
+        help="Return the input files of a task. Evaluates the file.",
         parents=[base_parser],
     )
+    subparser.set_defaults(command_function=main_get_inputs)
     subparser.add_argument(
         "--ignore",
         nargs="*",
         action="append",
         help="Specify file ignore patterns.",
     )
     subparser.add_argument("targets", nargs="+")
     add_threads_argument(subparser)
 
     ######## outputs
     subparser = subparsers.add_parser(
         "outputs",
-        help="Return the output files of a target. Evaluates the file.",
+        help="Return the output files of a task. Evaluates the file.",
         parents=[base_parser],
     )
+    subparser.set_defaults(command_function=main_get_outputs)
     subparser.add_argument(
         "--ignore",
         nargs="*",
         action="append",
         help="Specify file ignore patterns.",
     )
-    subparser.add_argument("targets", nargs="+")
+    subparser.add_argument("output_names", nargs="+")
+
     add_threads_argument(subparser)
 
     ######## evaluate
     subparser = subparsers.add_parser(
         "evaluate",
         help="Evaluate the specified Makex File (or paths with Makex Files) for the specified variable.",
         parents=[base_parser],
@@ -422,18 +434,20 @@
     subparser.add_argument(
         "variable_name",
         help="Name of the variable to evaluate. Can be target(name).* to evaluated variables of named targets  in the file.",
     )
 
     ######### targets subcommand
     subparser = subparsers.add_parser(
-        "targets",
+        "tasks",
+        aliases=["targets"], # TODO: remove this.
         parents=[base_parser],
         help="Generate list of targets parsed from the makex file found in path.",
     )
+    subparser.set_defaults(command_function=main_targets)
     subparser.add_argument(
         "path",
         nargs="?",
         help="Path to a makex file or directory. The current directory is the default.",
     )
     subparser.add_argument(
         "--paths",
@@ -450,84 +464,92 @@
     ######### completions command
     subparser = subparsers.add_parser(
         "completions",
         parents=[base_parser],
         description="Generate completion files for shells.",
         help="Generate completion files for shells.",
     )
+    subparser.set_defaults(command_function=main_completions)
+
     #if HAS_SHTAB:
     #    shtab.add_argument_to(
     #        subparser, option_string=["--shell"], parent=parser, preamble=PREAMBLE
     #    ) # magic!
     #else:
     subparser.add_argument("--shell", choices=["bash", "zsh"])
+    subparser.add_argument("--internal", action="store_true", default=False)
 
     subparser.add_argument(
         "file",
         nargs="?",
         help="The output file to write the completions to. If not specified, will the completion will be written to standard out.",
     )
 
     ######### workspace command
     subparser = subparsers.add_parser(
         "workspace",
         parents=[base_parser],
         description="Print the current workspace, or the workspace detected at path.",
         help="Print the current workspace, or the workspace detected at path.",
     )
+    subparser.set_defaults(command_function=main_workspace)
+
     subparser.add_argument(
         "path",
         nargs="?",
         help="Path representing a workspace, or inside a workspace.",
     )
 
     ######### complete command
     subparser = subparsers.add_parser(
         "complete",
         parents=[base_parser],
         help="Print completions for the specified input. This is used for shell completions.",
     )
+    subparser.set_defaults(command_function=main_complete)
+
     subparser.add_argument(
         "string",
         nargs="?",
         help="May be a complete/partial path. May include a target name.",
     )
 
     ######### version command
     subparser = subparsers.add_parser(
         "version",
         help="Print the makex version",
     )
+    subparser.set_defaults(command_function=main_version)
 
     return parser
 
 
+def _kill_running_processes():
+    # XXX: send a signal to any processes we created.
+    for pid in get_running_process_ids():
+        os.killpg(os.getpgid(pid), signal.SIGKILL)
+
+
 def _handle_signal_interrupt(_signal, frame):
     # TODO: attempt to shutdown pool gracefully
     # self.pool.shutdown()
     # self.pool.shutdown(cancel_futures=True)
     print('You pressed Ctrl+C or the process was interrupted!')
-
-    # XXX: send a signal to any processes we created.
-    for pid in get_running_process_ids():
-        os.killpg(os.getpgid(pid), signal.SIGKILL)
-
+    _kill_running_processes()
     sys.exit(-1)
 
 
 def _handle_signal_terminate(_signal, frame):
     # TODO: attempt to shutdown pool gracefully
     # self.pool.shutdown()
     # self.pool.shutdown(cancel_futures=True)
     print('You pressed Ctrl+C or the process was interrupted!')
 
-    # XXX: send a signal to any processes we created.
-    for pid in get_running_process_ids():
-        # send a kill because it's more reliable.
-        os.killpg(os.getpgid(pid), signal.SIGKILL)
+    # send a kill because it's more reliable.
+    _kill_running_processes()
 
     sys.exit(-1)
 
 
 def parse_scope(scope):
     type = None
     if scope.startswith("//"):
@@ -582,22 +604,20 @@
             if entry.name in names:
                 yield Path(entry.path, entry.name)
         elif entry.is_dir():
             yield from _find_files(entry, names)
 
 
 def find_makex_files(path, names):
-    checked = []
-    for file in path.iterdir():
-        if file.name in names:
-            return file, None
-        else:
-            checked.append(file)
+    for name in names:
+        file = path.joinpath(name)
+        if file.exists():
+            return file
 
-    return None, checked
+    return None
 
 
 def early_ui_printer(max_level: int, colors: ColorsNames):
     # we need an early ui before configuration/context is loaded
     def f(message, level=1, error=False):
         if error:
             print(f"{colors.ERROR}ERROR:{colors.RESET} {message}")
@@ -660,21 +680,26 @@
         # TODO: We need to strip the PATH too.
         current_enviroment.pop("VIRTUAL_ENV")
 
     if configuration.environment:
         early_ui(
             f"Evaluating environment from configuration: {configuration.environment}...", level=1
         )
-        configuration_environment = evaluate_configuration_environment(
-            shell=configuration.shell or Context.shell,
-            env=configuration.environment,
-            current_enviroment=current_enviroment,
-            cwd=cwd,
-            run=run,
-        )
+        try:
+            configuration_environment = evaluate_configuration_environment(
+                shell=configuration.shell or Context.shell,
+                env=configuration.environment,
+                current_enviroment=current_enviroment,
+                cwd=cwd,
+                run=run,
+            )
+        except ConfigurationError as e:
+            early_ui(e, error=True)
+            sys.exit(-1)
+
         if configuration_environment:
             early_ui(f"Environment from configuration: {configuration_environment}", level=1)
             current_enviroment.update(configuration_environment)
 
     argument = args.workspace if WORKSPACE_ARGUMENT_ENABLED else None
     workspace = current_workspace(
         cwd,
@@ -717,50 +742,53 @@
     """
     A variation of parse target which prints errors
     :param base:
     :param string:
     :param check:
     :return:
     """
+
     # resolve the path/makefile?:target_or_build_path name
     # return name/Path
     parts = string.split(":", 1)
     if len(parts) == 2:
         path, target = parts
         path = Path(path)
 
         if not target:
             ctx.ui.print(f"Invalid target name {target!r} in {string!r}.", error=True)
             sys.exit(-1)
 
         if path.parts and path.parts[0] == "//":
-            path = ctx.workspace_object.path / path
+            trace("Translate workspace path %s %s", path, ctx.workspace_object.path)
+            path = ctx.workspace_object.path.joinpath(*path.parts[1:])
         elif not path.is_absolute():
             path = base / path
-
-        if path.is_symlink():
+        elif path.is_symlink():
             path = path.readlink()
     else:
         target = parts[0]
         path = base
 
+    #trace("Parse target %s -> %s:%s %s %s", string, target, path, parts, path.parts)
     if path.is_dir():
+        #if check:
+        # check for Build/Makexfile in path
+        file = find_makex_files(path, names=ctx.makex_file_names)
+        if file is None:
+            ctx.ui.print(f"Makex file does not exist for target specified: {target}", error=True)
+            for check in ctx.makex_file_names:
+                ctx.ui.print(f"- Checked in {path/check}")
+            sys.exit(-1)
+    else:
+        if DIRECT_REFERENCES_TO_MAKEX_FILES is False:
+            raise Error(f"Path to target is not a directory. Got {path}.")
+        file = path
 
-        if check:
-            # check for Build/Makexfile in path
-            path, checked = find_makex_files(path, names=ctx.makex_file_names)
-            if path is None:
-                ctx.ui.print(
-                    f"Makex file does not exist for target specified: {target}", error=True
-                )
-                for check in checked:
-                    ctx.ui.print(f"- Checked in {check}")
-                sys.exit(-1)
-
-    return ResolvedTargetReference(target, path=path)
+    return ResolvedTargetReference(target, path=file)
 
 
 def main_clean(args, extra):
     """
     - Clean the specified targets in the makex file in the current working directory
     - (support recursive target specifier ... or //...)
     - or, clean all of them
@@ -839,29 +867,28 @@
     """
     Return build path of specified of target
     :param args:
     :return:
     """
     cwd = Path.cwd()
     ctx = init_context_standard(cwd, args)
-    ref = parse_target(ctx, cwd, args.target)
+    ref = parse_target(ctx, cwd, args.task)
 
     #debug("Current environment: %s", pformat(os.environ.__dict__, indent=2))
 
     if ref is None:
-        print(f"Invalid target reference: {args.target!r}")
+        print(f"Invalid task reference: {args.task!r}")
         sys.exit(-1)
 
     target_input = ref.path
 
     # assume the default/detected
     workspace = ctx.workspace_object
 
     if args.real:
-        # ignore all the other arguments because we're
         workspace = which_workspace(workspace.path, target_input)
 
     obj = get_build_path(
         objective_name=ref.name,
         variants=[],
         input_directory=target_input,
         build_root=ctx.cache,
@@ -892,15 +919,54 @@
 def main_get_outputs(args):
     """
     Return the output files of target/path (optionally recursively).
 
     :param args:
     :return:
     """
-    pass
+    cwd = Path.cwd()
+    ctx = init_context_standard(cwd, args)
+
+    target = parse_target(ctx, cwd, args.target)
+    ctx.graph = graph = TargetGraph()
+    ctx.ui.print(f"Current working directory: {ctx.colors.BOLD}{cwd}{ctx.colors.RESET}")
+
+    ctx.ui.print(f"Loading makex file at {target.path}")
+
+    result = parse_makefile_into_graph(ctx, target.path, graph)
+
+    if result.errors:
+        print_errors(ctx, result.errors)
+        sys.exit(-1)
+
+    t = graph.get_target(target)
+    if t is None:
+        ctx.ui.print(
+            f"Target \"{ctx.colors.BOLD}{target.name}{ctx.colors.RESET}\" not found in {target.path}",
+            error=True
+        )
+        sys.exit(-1)
+
+    # XXX: don't execute anything, evaluate the target outputs manually
+    executor = Executor(ctx, workers=1, force=args.force)
+    evaluated, errors = executor._evaluate_target(t)
+
+    if len(errors):
+        print_errors(ctx, errors)
+        sys.exit(-1)
+
+    if args.output_names:
+        paths = []
+        for output_name in args.output_names:
+            output = evaluated.outputs.get(output_name)
+            paths.append(output.path)
+        print(" ".join(paths))
+    else:
+        for output in evaluated.outputs:
+            print(output.path)
 
 
 def main_targets(args, extra_args):
     # Fast function to print targets of specified directory or makex file.
     cwd = Path.cwd()
 
     #if args.directory:
@@ -924,15 +990,15 @@
         else:
             _path = Path(path)
             if not _path.is_absolute():
                 _path = cwd / _path
     else:
         _path = cwd
 
-    file, _ = find_makex_files(_path, ctx.makex_file_names)
+    file = find_makex_files(_path, ctx.makex_file_names)
 
     if not file:
         return sys.exit(-1)
 
     ctx.graph = graph = TargetGraph()
 
     directory = file.parent
@@ -967,15 +1033,15 @@
     result = parse_makefile_into_graph(ctx, file, graph)
 
     for name, target in result.makex_file.targets.items():
         yield name, target
 
 
 def _find_makefile_and_yield(ctx, directory):
-    file, _ = find_makex_files(directory, ctx.makex_file_names)
+    file = find_makex_files(directory, ctx.makex_file_names)
 
     if not file:
         return None
 
     yield from _yield_targets(ctx, file, ctx.graph)
 
 
@@ -990,14 +1056,16 @@
 
     ctx = init_context_standard(cwd, args)
     print(ctx.workspace_path)
 
 
 def main_complete(args, extra_args):
     """
+    TODO: rename to shell-complete
+
     Complete the specified argument (path/target/etc).
 
     :param args:
     :param extra_args:
     :return:
     """
     # XXX: this is used in bash completions and should return fast/early.
@@ -1190,26 +1258,30 @@
         file = None
 
     output = sys.stdout
     if file:
         file.parent.mkdir(parents=True, exist_ok=True)
         output = file.open("w")
 
-    if HAS_SHTAB is False:
+    if args.internal is False and HAS_SHTAB is False:
         COMPLETIONS_PACKAGE = "makex.data.completions"
         resource_name = f"makex.{args.shell}"
         # load static completions from data directory
         if not importlib.resources.is_resource(COMPLETIONS_PACKAGE, resource_name):
             print(
                 f"Error: Could not find static shell script for {resource_name} in {COMPLETIONS_PACKAGE}."
             )
             sys.exit(-1)
         print(importlib.resources.read_text(COMPLETIONS_PACKAGE, resource_name), file=output)
         sys.exit(-1)
     else:
+        if HAS_SHTAB is False:
+            print("shtab is not installed. pip install shtab")
+            sys.exit(-1)
+
         from makex._shtab import PREAMBLE
         shell = args.shell
         _parser = parser(documentation=False)
         script = shtab.complete(_parser, shell=shell, preamble=PREAMBLE)
         print(script, file=output)
 
     return 0
@@ -1236,15 +1308,15 @@
 
     ctx = init_context_standard(cwd, args)
 
     #debug("Current environment: %s", pformat(os.environ.__dict__, indent=2))
 
     targets = []
 
-    for target in args.targets:
+    for target in args.tasks:
         ref = parse_target(ctx, cwd, target)
         targets.append(ref)
 
     ctx.graph = graph = TargetGraph()
     ctx.ui.print(f"Current working directory: {ctx.colors.BOLD}{cwd}{ctx.colors.RESET}")
     for target in targets:
 
@@ -1258,15 +1330,15 @@
 
     targets_to_run = []
 
     for target in targets:
         t = graph.get_target(target)
         if t is None:
             ctx.ui.print(
-                f"Target \"{ctx.colors.BOLD}{target.name}{ctx.colors.RESET}\" not in found in {target.path} {target}",
+                f"Target \"{ctx.colors.BOLD}{target.name}{ctx.colors.RESET}\" not found in {target.path}",
                 error=True
             )
             sys.exit(-1)
 
         targets_to_run.append(t)
 
     ctx.ui.print(f"Executing {len(targets_to_run)} targets...")
@@ -1285,14 +1357,19 @@
 
     # XXX: Currently set to one to avoid much breakage. Things are fast enough, for now.
     workers = 1 or args.threads
     executor = Executor(ctx, workers=workers, force=args.force)
 
     try:
         executed, errors = executor.execute_targets(*targets_to_run)
+    except KeyboardInterrupt as e:
+        executor.stop.set()
+        _kill_running_processes()
+        sys.exit(-1)
+
     except IOError as e:
         exc_info = sys.exc_info()
         traceback.print_exception(*exc_info)
         ctx.ui.print(f"There was an IO Error: {e} ({e.filename})", error=True)
         sys.exit(-1)
 
     except Exception as e:
@@ -1308,14 +1385,15 @@
     "run": main_run,
     "path": main_get_path,
     "targets": main_targets,
     "workspace": main_workspace,
     "complete": main_complete,
     "completions": main_completions,
     "version": main_version,
+    "outputs": main_get_outputs
 }
 
 
 def main():
     signal.signal(signal.SIGINT, _handle_signal_interrupt)
     signal.signal(signal.SIGTERM, _handle_signal_terminate)
 
@@ -1346,15 +1424,15 @@
             profiler.enable()
         elif args.profile_mode == "yappi":
             import yappi
             yappi.set_clock_type("cpu") # Use set_clock_type("wall") for wall time
             yappi.start()
 
     try:
-        COMMANDS[args.command.replace("-", "_")](args, extra_args)
+        args.command_function(args, extra_args)
     finally:
         if args.profile:
             if args.profile_mode == "cprofile":
                 profiler.disable()
             elif args.profile_mode == "yappi":
                 yappi.stop()
```

### Comparing `makex-20240203/python/makex/_logging.py` & `makex-20240401/python/makex/_logging.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,74 @@
 import logging
 import sys
+from functools import (
+    partial,
+    partialmethod,
+)
 from logging import StreamHandler
 
-LOGGER = logging.getLogger("makex")
+from makex.colors import (
+    BOLD,
+    RESET,
+    BLUE,
+    RED,
+    WHITE,
+    YELLOW,
+)
+
+debug = logging.debug
+error = logging.error
+info = logging.info
+warn = logging.warning
+warning = logging.warning
 
-#These are the sequences need to get colored ouput
-RESET_SEQ = "\033[0m"
-COLOR_SEQ = "\033[1;%dm"
-BOLD_SEQ = "\033[1m"
+# hack in a new trace level https://stackoverflow.com/a/55276759
+logging.TRACE = 5
+logging.addLevelName(logging.TRACE, 'TRACE')
+logging.Logger.trace = partialmethod(logging.Logger.log, logging.TRACE)
+logging.trace = partial(logging.log, logging.TRACE)
 
-BLACK, RED, GREEN, YELLOW, BLUE, MAGENTA, CYAN, WHITE = [30 + r for r in range(8)]
-COLORS = {
+trace = logging.trace
+
+LOGGER = logging.getLogger("makex")
+
+COLOR_SEQUENCES = {
     logging.WARNING: YELLOW,
     logging.INFO: WHITE,
     logging.DEBUG: BLUE,
-    logging.CRITICAL: YELLOW,
-    logging.ERROR: RED
-}
-
-COLOR_SEQUENCS = {
-    logging.WARNING: COLOR_SEQ % YELLOW,
-    logging.INFO: COLOR_SEQ % WHITE,
-    logging.DEBUG: COLOR_SEQ % BLUE,
-    logging.CRITICAL: COLOR_SEQ % YELLOW,
-    logging.ERROR: COLOR_SEQ % RED
+    logging.CRITICAL: RED,
+    logging.ERROR: RED,
+    logging.TRACE: WHITE,
 }
 
 
 class ColoredStream(logging.StreamHandler):
     def __init__(
         self,
-        fmt="%(COLOR)s[%(levelname)s]%(RESET)s[%(BOLD)s%(name)s%(RESET)s] (%(BOLD)s%(filename)s%(RESET)s:%(lineno)d) %(message)s",
-        colors=COLORS,
+        fmt="%(COLOR)s[makex][%(levelname)s]%(RESET)s[%(BOLD)s%(name)s%(RESET)s] (%(BOLD)s%(filename)s%(RESET)s:%(lineno)d) %(message)s",
+        colors=COLOR_SEQUENCES,
     ):
         super().__init__()
         self.colors = colors
         self.formatter = logging.Formatter(fmt)
 
     def emit(self, record: logging.LogRecord) -> None:
-        level_color = self.colors.get(record.levelno, False)
-        level_color = COLOR_SEQ % level_color if level_color else ""
+        level_color = self.colors.get(record.levelno, "")
+        #level_color = COLOR_SEQ % level_color if level_color else "
+
         record.__dict__["COLOR"] = level_color
-        record.__dict__["BOLD"] = BOLD_SEQ
-        record.__dict__["RESET"] = RESET_SEQ
+        record.__dict__["BOLD"] = BOLD
+        record.__dict__["RESET"] = RESET
 
         print(self.formatter.format(record))
 
 
 def initialize_logging(color=False, level=logging.NOTSET):
     logger = logging.getLogger()
 
-    #if level:
-    #    logging.basicConfig(level=level)
-
     for handler in logger.handlers:
         logger.removeHandler(handler)
 
     if level:
         if color:
             logger.addHandler(ColoredStream())
         else:
@@ -64,29 +76,7 @@
                 fmt="[%(levelname)s][%(name)s] (%(filename)s:%(lineno)d) %(message)s "
             )
             handler = StreamHandler(sys.stdout)
             handler.setLevel(level)
             handler.setFormatter(fmt)
             logger.addHandler(handler)
         logger.setLevel(level)
-
-
-debug = logging.debug
-error = logging.error
-info = logging.info
-warn = logging.warning
-warning = logging.warning
-#addLoggingLevel("TRACE", logging.DEBUG -5)
-
-import logging
-from functools import (
-    partial,
-    partialmethod,
-)
-
-# hack in a new trace level https://stackoverflow.com/a/55276759
-logging.TRACE = 5
-logging.addLevelName(logging.TRACE, 'TRACE')
-logging.Logger.trace = partialmethod(logging.Logger.log, logging.TRACE)
-logging.trace = partial(logging.log, logging.TRACE)
-
-trace = logging.trace
```

### Comparing `makex-20240203/python/makex/_shtab.py` & `makex-20240401/python/makex/_shtab.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 """
 - Modify fix shtab so it handles colon characters (use _get_comp_words_by_ref for completing word variable).
 - Set IFS for the entire run.
 
 """
+import sys
 from string import Template
 
 try:
     from shtab import (
         get_bash_commands,
         mark_completer,
         wordify,
     )
 except ImportError as e:
-    pass
-
-
+    print("shtab is not installed. pip install shtab")
+    sys.exit(-1)
 
 TEMPLATE = """# AUTOMATICALLY GENERATED by `shtab`
 
 ${subparsers}
 
 ${option_strings}
 
@@ -185,15 +185,14 @@
             "\n# Custom Preamble\n" + preamble + "\n# End Custom Preamble\n" if preamble else ""
         ),
         root_prefix=root_prefix,
         prog=parser.prog,
     )
 
 
-
 # yapf: disable
 PREAMBLE = {
     "bash": r"""
 # $1=COMP_WORDS[1]
 _shtab_makex_compgen_paths() {
     makex complete ${1}
 }
@@ -208,8 +207,8 @@
   compadd -a - plugins
   #  -M 'r:|=*'
   #makex complete "$curcontext"
 }   
 """,
     "tcsh": "",
 }
-# yapf: enable
+# yapf: enable
```

### Comparing `makex-20240203/python/makex/api.py` & `makex-20240401/python/makex/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 class Help:
     url: str
     text: str
     markdown: str
     html: str
 
 
-class Runnable:
+class Action:
     def help(self):
         # return help documents
         pass
 
     def arguments(self):
-        # return the arguments the runnable takes, in order, but also named for keyword arguments.
+        # return the arguments the Action takes, in order, but also named for keyword arguments.
         # handle different types automatically like, list of path, path, dict[str], etc
         pass
 
     def run(self, ctx: Context, target: Target):
         # do whatever is required to run
         pass
```

### Comparing `makex-20240203/python/makex/build_path.py` & `makex-20240401/python/makex/build_path.py`

 * *Files 0% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
     if linkpath is None:
         return
 
     if linkpath.exists():
         if not linkpath.is_symlink():
             raise Exception(
-                f"Linkpath {linkpath} exists, but it is not a symlink. Output directory may have been created inadvertantly outside the tool."
+                f"Linkpath {linkpath} exists, but it is not a symlink. Output directory may have been created inadvertently outside the tool."
             )
     else:
         if linkpath.exists() is False and linkpath.is_symlink():
             # we have a broken symlink
             if fix:
                 realpath = linkpath.readlink().absolute()
                 logging.debug("Fixing broken link from %s to %s", linkpath, realpath)
@@ -461,15 +461,15 @@
 
         if debug:
             print(f"Link from {source_path } to {linkpath}")
 
         if linkpath.exists():
             if not linkpath.is_symlink():
                 raise Exception(
-                    f"Linkpath {linkpath} exists, but it is not a symlink. Build directory may have been created inadvertantly outside the use of build-tool."
+                    f"Linkpath {linkpath} exists, but it is not a symlink. Build directory may have been created inadvertently outside the use of build-tool."
                 )
         else:
             linkpath.symlink_to(source_path)
 
         print((Path(linkpath) / objective)) # / working_folder))
     else:
         print(new_path)
```

### Comparing `makex-20240203/python/makex/configuration.py` & `makex-20240401/python/makex/configuration.py`

 * *Files 12% similar despite different names*

```diff
@@ -28,29 +28,29 @@
 
 class ConfigurationError(MakexError):
     def __init__(self, message, location: GenericFileLocation):
         super().__init__(message)
         self.location = location
 
 
-class ConfigurationStringValue(str):
+class ConfigurationValue:
     """
         Track string value locations because they are usually a source of problems, and we want to refer to that location
         for the user.
     """
     def __init__(self, value, location: GenericFileLocation = None):
         super().__init__()
         self.value = value
         self.location = location
 
     #def __str__(self):
     #    return self.value
 
-    def __new__(cls, *args, **kwargs):
-        return super().__new__(cls, args[0])
+    #def __new__(cls, *args, **kwargs):
+    #    return super().__new__(cls, args[0])
 
 
 @dataclass
 class Configuration:
     path: Path = None
 
     workspace: str = None
@@ -93,17 +93,16 @@
             output_folder = root.get("output_folder", None)
         else:
             output_folder = None
 
         environment = root.get("environment", {})
 
         environment = {
-            k: ConfigurationStringValue(v, GenericFileLocation(path))
-            for k,
-            v in environment.items()
+            k: ConfigurationValue(v, GenericFileLocation(path))
+            for k, v in environment.items()
         }
         return cls(
             path=path,
             workspace=workspace,
             cache=cache,
             shell=shell,
             file_names=file_names,
@@ -177,38 +176,51 @@
     env: dict[str, str],
     current_enviroment: dict[str, str],
     cwd,
     run: RunFunction,
 ) -> dict[str, str]:
     d = {}
     for k, v in env.items():
-        if v.startswith(SHELL_MARKER):
-            script = v[len(SHELL_MARKER):]
+        value = v.value
 
-            read, write = os.pipe()
-            os.write(write, script.encode("utf-8"))
-            os.close(write)
-
-            process = run(
-                shell,
-                env=current_enviroment,
-                capture=True,
-                shell=False,
-                print=False,
-                cwd=cwd,
-                stdin=read,
-            )
-            if process.status != 0:
-                location: GenericFileLocation = getattr(v, "location", None)
-                raise ConfigurationError(
-                    f"Invalid shell command when evaluating environment variables from the file {location.path}.",
-                    location=location
+        if isinstance(value, dict):
+            script = value.get("shell", None)
+            if script is not None:
+
+                read, write = os.pipe()
+                os.write(write, script.encode("utf-8"))
+                os.close(write)
+                print(shell, script)
+                process = run(
+                    shell,
+                    env=current_enviroment,
+                    capture=True,
+                    shell=False,
+                    print=False,
+                    cwd=cwd,
+                    stdin=read,
                 )
-            # XXX: newline is removed so paths evaluate easy
-            v = process.output.strip("\n")
+                if process.status != 0:
+                    location: GenericFileLocation = getattr(v, "location", None)
+                    raise ConfigurationError(
+                        f"Invalid shell command when evaluating environment variables from the file {location.path}:\n\t{value}\n:{process.output}\n{process.error}",
+                        location=location
+                    )
+                # XXX: newline is removed so paths evaluate easy
+                v = process.output.strip("\n")
+        elif isinstance(value, str):
+            pass
+        elif isinstance(value, bool):
+            value = "1" if value else "0"
+        else:
+            raise ConfigurationError(
+                f"Invalid environment variable value type {type(value)} for {k} when evaluating environment variables from the file {value.location.path}:\n\t{v}",
+                location=value.location
+            )
+
         d[k] = v
 
     return d
 
 
 @dataclass
 class ConfigurationFiles:
```

### Comparing `makex-20240203/python/makex/context.py` & `makex-20240401/python/makex/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,17 +33,18 @@
 from makex.ui import UI
 from makex.workspace import (
     Workspace,
     WorkspaceCache,
 )
 
 if BUILT_IN_REFLINKS:
-    import makex.reflink as reflink
+    import makex.file_cloning as reflink
 else:
-    import reflink
+    import file_cloning
+
 
 @dataclass
 class Context:
     """
     Define a generic context so that subclasses can be defined with properties with types local to the subclass.
 
     TODO: copy the values so they are all private self.__dict__[fqn.].
```

### Comparing `makex-20240203/python/makex/data/completions/makex.bash` & `makex-20240401/python/makex/data/completions/makex.bash`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 # AUTOMATICALLY GENERATED by `shtab`
 
-_shtab_makex_subparsers=('run' 'path' 'dot' 'affected' 'inputs' 'outputs' 'evaluate' 'targets' 'completions' 'workspace' 'complete' 'version')
+_shtab_makex_subparsers=('run' 'path' 'dot' 'affected' 'inputs' 'outputs' 'evaluate' 'tasks' 'targets' 'completions' 'workspace' 'complete' 'version')
 
 _shtab_makex_option_strings=('-h' '--help' '--verbose' '--debug' '--color' '--cache')
 _shtab_makex_run_option_strings=('-h' '--help' '--directory' '--force' '--dry' '--threads')
 _shtab_makex_path_option_strings=('-h' '--help' '--real')
 _shtab_makex_dot_option_strings=('-h' '--help' '--files' '--ignore' '--threads')
 _shtab_makex_affected_option_strings=('-h' '--help' '--threads')
 _shtab_makex_inputs_option_strings=('-h' '--help' '--ignore' '--threads')
 _shtab_makex_outputs_option_strings=('-h' '--help' '--ignore' '--threads')
 _shtab_makex_evaluate_option_strings=('-h' '--help')
+_shtab_makex_tasks_option_strings=('-h' '--help' '--paths' '--prefix')
 _shtab_makex_targets_option_strings=('-h' '--help' '--paths' '--prefix')
-_shtab_makex_completions_option_strings=('-h' '--help' '--shell')
+_shtab_makex_completions_option_strings=('-h' '--help' '--shell' '--internal')
 _shtab_makex_workspace_option_strings=('-h' '--help')
 _shtab_makex_complete_option_strings=('-h' '--help')
 _shtab_makex_version_option_strings=('-h' '--help')
 
 _shtab_makex_run_pos_0_COMPGEN=_shtab_makex_compgen_paths
 
-_shtab_makex_pos_0_choices=('run' 'path' 'dot' 'affected' 'inputs' 'outputs' 'evaluate' 'targets' 'completions' 'workspace' 'complete' 'version')
+_shtab_makex_pos_0_choices=('run' 'path' 'dot' 'affected' 'inputs' 'outputs' 'evaluate' 'tasks' 'targets' 'completions' 'workspace' 'complete' 'version')
 _shtab_makex___profile_mode_choices=('cprofile' 'yappi')
 _shtab_makex___color_choices=('off' 'auto' 'on')
 _shtab_makex_run___profile_mode_choices=('cprofile' 'yappi')
 _shtab_makex_run___color_choices=('off' 'auto' 'on')
 _shtab_makex_path___profile_mode_choices=('cprofile' 'yappi')
 _shtab_makex_path___color_choices=('off' 'auto' 'on')
 _shtab_makex_dot___profile_mode_choices=('cprofile' 'yappi')
@@ -31,14 +32,17 @@
 _shtab_makex_affected___color_choices=('off' 'auto' 'on')
 _shtab_makex_inputs___profile_mode_choices=('cprofile' 'yappi')
 _shtab_makex_inputs___color_choices=('off' 'auto' 'on')
 _shtab_makex_outputs___profile_mode_choices=('cprofile' 'yappi')
 _shtab_makex_outputs___color_choices=('off' 'auto' 'on')
 _shtab_makex_evaluate___profile_mode_choices=('cprofile' 'yappi')
 _shtab_makex_evaluate___color_choices=('off' 'auto' 'on')
+_shtab_makex_tasks___profile_mode_choices=('cprofile' 'yappi')
+_shtab_makex_tasks___color_choices=('off' 'auto' 'on')
+_shtab_makex_tasks___paths_choices=('absolute' 'workspace' 'relative' 'None')
 _shtab_makex_targets___profile_mode_choices=('cprofile' 'yappi')
 _shtab_makex_targets___color_choices=('off' 'auto' 'on')
 _shtab_makex_targets___paths_choices=('absolute' 'workspace' 'relative' 'None')
 _shtab_makex_completions___profile_mode_choices=('cprofile' 'yappi')
 _shtab_makex_completions___color_choices=('off' 'auto' 'on')
 _shtab_makex_completions___shell_choices=('bash' 'zsh')
 _shtab_makex_workspace___profile_mode_choices=('cprofile' 'yappi')
@@ -86,23 +90,29 @@
 _shtab_makex_outputs___verbose_nargs=0
 _shtab_makex_outputs___debug_nargs=0
 _shtab_makex_outputs___ignore_nargs=*
 _shtab_makex_evaluate__h_nargs=0
 _shtab_makex_evaluate___help_nargs=0
 _shtab_makex_evaluate___verbose_nargs=0
 _shtab_makex_evaluate___debug_nargs=0
+_shtab_makex_tasks__h_nargs=0
+_shtab_makex_tasks___help_nargs=0
+_shtab_makex_tasks___verbose_nargs=0
+_shtab_makex_tasks___debug_nargs=0
+_shtab_makex_tasks___prefix_nargs=0
 _shtab_makex_targets__h_nargs=0
 _shtab_makex_targets___help_nargs=0
 _shtab_makex_targets___verbose_nargs=0
 _shtab_makex_targets___debug_nargs=0
 _shtab_makex_targets___prefix_nargs=0
 _shtab_makex_completions__h_nargs=0
 _shtab_makex_completions___help_nargs=0
 _shtab_makex_completions___verbose_nargs=0
 _shtab_makex_completions___debug_nargs=0
+_shtab_makex_completions___internal_nargs=0
 _shtab_makex_workspace__h_nargs=0
 _shtab_makex_workspace___help_nargs=0
 _shtab_makex_workspace___verbose_nargs=0
 _shtab_makex_workspace___debug_nargs=0
 _shtab_makex_complete__h_nargs=0
 _shtab_makex_complete___help_nargs=0
 _shtab_makex_complete___verbose_nargs=0
```

### Comparing `makex-20240203/python/makex/data/completions/makex.zsh` & `makex-20240401/python/makex/data/completions/makex.zsh`

 * *Files 3% similar despite different names*

```diff
@@ -8,17 +8,18 @@
     "affected:"
     "complete:"
     "completions:Generate completion files for shells."
     "dot:"
     "evaluate:"
     "inputs:"
     "outputs:"
-    "path:Get the output path of a target."
-    "run:Run a target or list of targets."
+    "path:Get the output path of a task."
+    "run:Run a task or list of tasks."
     "targets:"
+    "tasks:"
     "version:"
     "workspace:Print the current workspace, or the workspace detected at path."
   )
   _describe 'makex commands' _commands
 }
 
 _shtab_makex_options=(
@@ -39,14 +40,15 @@
   "(- : *)"{-h,--help}"[show this help message and exit]"
   ":May be a complete\/partial path. May include a target name.:"
 )
 
 _shtab_makex_completions_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
   "--shell[]:shell:(bash zsh)"
+  "--internal[]"
   ":The output file to write the completions to. If not specified, will the completion will be written to standard out.:"
 )
 
 _shtab_makex_dot_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
   "--files[Include\/evaluate files\/globs. May be slow.]:files:"
   "*--ignore[Specify file ignore patterns for input\/output files.]:ignore:"
@@ -67,39 +69,46 @@
   "(*):targets:"
 )
 
 _shtab_makex_outputs_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
   "*--ignore[Specify file ignore patterns.]:ignore:"
   "--threads[Worker threads to spawn for running\/evaluating targets in parallel. Automatically detected.]:threads:"
-  "(*):targets:"
+  "(*):output_names:"
 )
 
 _shtab_makex_path_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
   "--real[Return cache path. This may be slower as it must resolve Workspaces.]"
-  ":Name and optional path of a target. \/\/path\:name, \/\/\:name, \:name are all valid.:"
+  ":Name and optional path of a task. \/\/path\:name, \/\/\:name, \:name are all valid.:"
 )
 
 _shtab_makex_run_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
-  "--directory[Change to directory before evaluating targets.]:directory:"
-  "--force[Always run all targets even if they don\'t need to be.]"
+  "--directory[Change to directory before evaluating tasks.]:directory:"
+  "--force[Always run all task even if they don\'t need to be.]"
   "--dry[Do a dry run. Nothing will be executed.]"
   "--threads[Worker threads to spawn for running\/evaluating targets in parallel. Automatically detected.]:threads:"
-  "(*):targets:_shtab_makex_complete_target"
+  "(*):tasks:_shtab_makex_complete_target"
 )
 
 _shtab_makex_targets_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
   "--paths[Path to a makex file or directory]:paths:(absolute workspace relative None)"
   "--prefix[]"
   ":Path to a makex file or directory. The current directory is the default.:"
 )
 
+_shtab_makex_tasks_options=(
+  "(- : *)"{-h,--help}"[show this help message and exit]"
+  "--paths[Path to a makex file or directory]:paths:(absolute workspace relative None)"
+  "--prefix[]"
+  ":Path to a makex file or directory. The current directory is the default.:"
+)
+
 _shtab_makex_version_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
 )
 
 _shtab_makex_workspace_options=(
   "(- : *)"{-h,--help}"[show this help message and exit]"
   ":Path representing a workspace, or inside a workspace.:"
@@ -126,14 +135,15 @@
         dot) _arguments -C -s $_shtab_makex_dot_options ;;
         evaluate) _arguments -C -s $_shtab_makex_evaluate_options ;;
         inputs) _arguments -C -s $_shtab_makex_inputs_options ;;
         outputs) _arguments -C -s $_shtab_makex_outputs_options ;;
         path) _arguments -C -s $_shtab_makex_path_options ;;
         run) _arguments -C -s $_shtab_makex_run_options ;;
         targets) _arguments -C -s $_shtab_makex_targets_options ;;
+        tasks) _arguments -C -s $_shtab_makex_tasks_options ;;
         version) _arguments -C -s $_shtab_makex_version_options ;;
         workspace) _arguments -C -s $_shtab_makex_workspace_options ;;
       esac
   esac
 }
 
 # Custom Preamble
@@ -149,8 +159,16 @@
   #makex complete "$curcontext"
 }
 
 # End Custom Preamble
 
 
 typeset -A opt_args
-_shtab_makex "$@"
+
+if [[ $zsh_eval_context[-1] == eval ]]; then
+  # eval/source/. command, register function for later
+  compdef _shtab_makex -N makex
+else
+  # autoload from fpath, call function directly
+  _shtab_makex "$@"
+fi
+
```

### Comparing `makex-20240203/python/makex/errors.py` & `makex-20240401/python/makex/errors.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 @dataclass(frozen=True)
 class GenericFileLocation:
     path: Path
     line: int = None
     column: int = None
 
 
-class GenericSyntaxError(Exception):
+class GenericSyntaxError(MakexError):
     def __init__(
         self, error: Union[str, Exception], location: GenericFileLocation, type, context=(1, 2)
     ):
         super().__init__(error)
         self.error = error
         self.location = location
         self.context = context
```

### Comparing `makex-20240203/python/makex/executor.py` & `makex-20240401/python/makex/executor.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 import logging
-import os
-import signal
 import threading
 import time
 from collections import deque
 from concurrent.futures import (
     Future,
     ThreadPoolExecutor,
 )
@@ -23,56 +21,54 @@
     trace,
     warning,
 )
 from makex.constants import (
     DATABASE_ENABLED,
     DATABASE_FILE_NAME,
     REMOVE_CACHE_DIRTY_TARGETS_ENABLED,
+    STORE_TASK_HASH_IN_OUTPUT_FILES,
     SYMLINK_PER_TARGET_ENABLED,
 )
 from makex.context import Context
 from makex.errors import (
     ExecutionError,
-    MakexError,
-    MissingInputFileError,
-    MissingOutputFileError,
     MultipleErrors,
 )
 from makex.file_checksum import FileChecksum
-from makex.make_file import (
-    FindFiles,
-    Glob,
-    InternalRunnableBase,
-    ListTypes,
+from makex.makex_file import (
+    InternalActionBase,
     MakexFileCycleError,
-    PathElement,
-    PathObject,
-    ResolvedTargetReference,
     TargetObject,
-    TargetReferenceElement,
-    _resolve_pathlike,
     find_makex_files,
     resolve_find_files,
     resolve_glob,
     resolve_path_element_workspace,
     resolve_string_path_workspace,
     resolve_target_output_path,
 )
+from makex.makex_file_types import (
+    FindFiles,
+    Glob,
+    ListTypes,
+    PathElement,
+    PathObject,
+    ResolvedTargetReference,
+    TargetReferenceElement,
+)
 from makex.metadata_sqlite import SqliteMetadataBackend
 from makex.protocols import FileStatus
 from makex.python_script import (
     FileLocation,
     PythonScriptError,
     StringValue,
 )
-from makex.run import get_running_process_ids
 from makex.target import (
     EvaluatedTarget,
     EvaluatedTargetGraph,
-    InternalRunnable,
+    InternalAction,
     TargetKey,
     brief_target_name,
 )
 
 
 class TargetResult:
     target: TargetObject
@@ -81,14 +77,75 @@
 
     def __init__(self, target, output=None, errors=None):
         self.target = target
         self.output = output or ""
         self.errors = errors or []
 
 
+_XATTR_OUTPUT_TARGET_HASH = b"user.makex.target_hash"
+
+from os import (
+    getxattr,
+    removexattr,
+    setxattr,
+)
+
+
+def _get_xattr(path, attribute: bytes):
+    try:
+        return getxattr(path, attribute)
+    except OSError as e:
+        if e.errno == 61:
+            return b""
+        raise e
+
+
+def _set_xattr(path, attribute: bytes, value: bytes):
+    return setxattr(path, attribute, value)
+
+
+def _remove_xattr(path, attribute):
+    return removexattr(path, attribute)
+
+
+def figure_out_location(obj, default):
+    location = getattr(obj, "location", None)
+
+    if location and isinstance(location, FileLocation):
+        return location
+    else:
+        location = None
+
+    if location is None: # or isinstance(obj, FileLocation) is False:
+        return default
+
+    return location
+
+
+# TODO: this method should be moved to the makex file module. _resolve_pathlike() fits the bill.
+def _transform_output_to_path(
+    ctx, target, base: Path, value: Union[StringValue, PathElement, PathObject]
+) -> Path:
+    # TODO: we probably won't get any StringValues as they are transformed earlier
+    if isinstance(value, StringValue):
+        path = resolve_string_path_workspace(ctx, target.workspace, value, base)
+    elif isinstance(value, PathElement):
+        # TODO: we should use the resolved path here
+        path = resolve_path_element_workspace(ctx, target.workspace, value, base)
+    elif isinstance(value, PathObject):
+        return value.path
+    else:
+        raise NotImplementedError(f"Invalid output type {type(value)}: {value!r}")
+
+    return path
+
+
+ExecuteResult = tuple[list[EvaluatedTarget], deque[Exception]]
+
+
 class Executor:
     # pool of threads and work queue
     pool: ThreadPoolExecutor
 
     # collect errors because the way concurrent.Futures swallows them
     errors: deque[Exception]
 
@@ -110,26 +167,28 @@
     # keep a cache of Target hashes because it's slightly expensive
     _hash_cache: dict[TargetKey, str]
 
     # our output (and state)
     graph_2: EvaluatedTargetGraph
 
     # queue of object we need to write to database. doing this because of sqlite issues...
-    # sqlite objects can't be accessed from different thread, so we'd need to recreate connections per each, or,
+    # sqlite objects can't be accessed from a different thread, so we'd need to recreate connections per each, or,
     # keep a queue.
     _database_queue: deque[EvaluatedTarget]
 
+    _executed_keys: set[str]
+
     def __init__(self, ctx: "Context", workers=1, force=False):
         self.ctx = ctx
         self._workers = workers
         self.force = force
         self.analysis_mode = False
 
         # our input
-        self.graph_1 = ctx.graph
+        self._graph_1 = ctx.graph
 
         self.stop = threading.Event()
 
         self._target_hash = {}
 
         self._disk_metadata = SqliteMetadataBackend(ctx.cache / DATABASE_FILE_NAME)
 
@@ -145,18 +204,18 @@
 
         self._reset()
 
     def _load_target_metadata(self, target: TargetObject) -> EvaluatedTarget:
         # load target information from metadata
         pass
 
-    def are_dependencies_executed(self, check_target: ResolvedTargetReference):
+    def _are_dependencies_executed(self, check_target: ResolvedTargetReference):
         try:
             # we don't need to use the cycle checking get_requires here because they've already been loaded into the graph.
-            requires = self.graph_1.get_requires(check_target)
+            requires = self._graph_1.get_requires(check_target)
         except MakexFileCycleError as e:
             self.errors.append(e)
             self.stop.set()
             return False
 
         if True:
             requires = list(requires)
@@ -164,35 +223,38 @@
 
         statuses = []
         for target in requires:
             statuses.append(self._target_status.get(target.key(), False))
 
         return all(statuses)
 
-    ExecuteResult = tuple[list[EvaluatedTarget], deque[Exception]]
-
     def _reset(self):
         self._database_queue = deque()
         self.graph_2 = EvaluatedTargetGraph()
         self.pool = ThreadPoolExecutor(self._workers)
         self.finished = []
         self.queued = deque()
         self.errors = deque()
         self.waiting = deque()
         self.stop.clear()
 
         self._target_status = {}
 
-        # keep the target hashes around for the life of the Executor
+        # keep the target hashes around for the life of the Executor. Uncomment for development.
         #self._target_hash = {}
 
         # XXX: must be reset every time we run an execute. Hashes of specific keys may change between runs.
         self._hash_cache = {}
 
+        self._executed_keys = set()
+
     def _store_database(self, target):
+        if self.ctx.dry_run:
+            return
+
         if DATABASE_ENABLED:
             key = target.key()
             hash = self._get_target_hash(target)
             trace("Storing target in database %s (%s)", key, hash)
             self._disk_metadata.put_target(key, hash)
 
     def execute_targets(self, *targets: TargetObject) -> ExecuteResult:
@@ -201,15 +263,14 @@
         This will block/loop in a thread until all the targets are finished.
 
         :param targets: A list of TargetObjects as provided by the Makex file parsing.
         :param force:
         :return:
         """
         # returns a list of targets finished/completed and any errors/exceptions
-        #self.finished = deque()
         self._reset()
 
         targets = list(targets)
 
         debug("Execute %s targets: %r...", len(targets), targets[:max(3, len(targets))])
         # execute targets in parallel
         # do a dfs for each
@@ -221,32 +282,28 @@
                 target.name, Path(target.makex_file_path), target.location
             )
             if len(target.requires) == 0:
                 # execute immediately. no requirements.
                 evaluated, errors = self._execute_target(target)
                 if errors:
                     return self.finished, errors
-
             #elif self.are_dependencies_executed(resolved_target):
             # execute immediately. all dependencies are resolved.
             # all dependencies of target are already executed.
             #trace("Execute initial")
             #    self._execute_target(target)
             else:
-                # if not isinstance(target, TargetObject):
-                #     raise ValueError(f"Invalid target:{target}: {type(target)} {target!r}")
-
-                # add the depedencies of target first, in order
+                # add the dependencies of target first, in order
                 # add to waiting so we can fetch them later
                 if True:
                     # CODE DUPLICATION
                     trace("Queue recursive deps of %s", resolved_target)
                     try:
                         # add all the possible requirements to waiting queue
-                        for req in self.graph_1.get_requires_detect_cycles(
+                        for req in self._graph_1.get_requires_detect_cycles(
                             resolved_target, recursive=True
                         ):
                             trace("Add to waiting %r", req)
                             self.waiting.append(req)
                     except MakexFileCycleError as e:
                         return [], [e]
 
@@ -264,61 +321,61 @@
                     self.stop.set()
                     continue
 
                 while len(self.queued) == self._workers:
                     #trace("Queue wait")
                     time.sleep(0.1)
 
+                if self.errors:
+                    debug("Execution had errors. Stopping")
+                    break
+
                 #target = self.waiting.pop(0)
                 target = self.waiting.popleft()
                 debug("Pop waiting %s: %s", target, target.key())
 
                 if target.key() in self.queued:
                     # Target has been already queued for execution. Wait until it is done.
-                    #print("target queued. skip", target)
+                    debug("target queued. skip: %s", target.key())
                     continue
 
                 if isinstance(target, ResolvedTargetReference):
-                    resolved_target = self.graph_1.get_target(target)
+                    resolved_target = self._graph_1.get_target(target)
 
                     if resolved_target is None:
                         #raise Exception(f"Could not find target {target.name} in file {target.path}: {target.location}")
                         self.errors.append(
                             ExecutionError(
                                 f"Could not find target {target.name} in file {target.path}",
                                 target,
                                 target.location
                             )
                         )
                         self.stop.set()
                         break
 
                     target = resolved_target
-                    #target =
-                    #assert target
 
                 if not target.requires:
                     # Target has no requirements, execute immediately.
                     evaluated, errors = self._execute_target(target)
 
                     if errors:
                         self.errors.extend(errors)
                         self.stop.set()
                 else:
                     resolved_target = ResolvedTargetReference(
                         target.name, Path(target.makex_file_path), target.location
                     )
-                    if self.are_dependencies_executed(resolved_target):
-                        #print("!!!exec target", target)
+                    if self._are_dependencies_executed(resolved_target):
                         evaluated, errors = self._execute_target(target)
                         if errors:
                             self.errors.extend(errors)
                             self.stop.set()
                     else:
-                        #print("make waiting again", target, target.requires)
                         # there may be errors during dependency checking
                         trace("Add back to waiting %r", target)
                         self.waiting.append(target)
                 i += 1
                 #if i == 5:
                 #    print("early break")
                 #    break
@@ -349,45 +406,46 @@
     def _checksum_file(self, path: Path) -> FileChecksum:
         if self._supports_extended_attribute is False:
             # we need to store the checksum in a database sidecar
             # store the checksum in the database
             if DATABASE_ENABLED is False:
                 raise NotImplementedError("No where to store file checksum.")
 
-            fingerprint = FileChecksum.fingerprint(path)
+            fingerprint = FileChecksum.get_fingerprint(path)
 
             string_path = str(path)
 
             checksum = self._disk_metadata.get_file_checksum(string_path, fingerprint)
 
             if checksum is None:
                 # db doesn't have checksum. create one and store it.
                 checksum = FileChecksum.make(path, fingerprint)
                 self._disk_metadata.put_file(
                     string_path,
                     fingerprint=checksum.fingerprint,
-                    checksum_type=checksum.type,
+                    checksum_type=checksum.type.value,
                     checksum=checksum.value,
                 )
         else:
             # filechecksum class handles the caching part
             checksum = FileChecksum.create(path)
         return checksum
 
     def _is_checksum_stale(self, path, checksum: FileChecksum = None):
         if False:
             status = self.metadata.get_file_status(path)
             if status.checksum == checksum:
                 return False
 
         if self._supports_extended_attribute is False:
+            # XXX: FS doesn't support xattr. Use the database to store/retrieve checksums.
             if DATABASE_ENABLED is False:
                 raise NotImplementedError("No where to check file checksum validity.")
 
-            fingerprint = FileChecksum.fingerprint(path)
+            fingerprint = FileChecksum.get_fingerprint(path)
             string_path = str(path)
 
             database_checksum = self._disk_metadata.get_file_checksum(string_path, fingerprint)
             if database_checksum is None:
                 return True
 
             if checksum != database_checksum:
@@ -399,14 +457,24 @@
             return FileChecksum.is_fingerprint_valid(path) is False
 
     def _create_output_link(self, target: EvaluatedTarget, cache: Path, fix=False):
         # TODO: optimize this upwards so it isn't called for each target. or use a filesystem cache
         # link from src() / "_output_" to cache
         linkpath = target.input_path / self.ctx.output_folder_name
         new_path = cache
+        debug(
+            "Symlink %s [exists=%s,symlink=%s] <- %s [exists=%s,symlink=%s]",
+            new_path,
+            new_path.exists(),
+            new_path.is_symlink(),
+            linkpath,
+            linkpath.exists(),
+            linkpath.is_symlink()
+        )
+
         if linkpath.exists():
             if not linkpath.is_symlink():
                 raise Exception(
                     f"Linkpath {linkpath} exists, but it is not a symlink. "
                     f"Output directory may have been created inadvertantly outside the tool."
                 )
 
@@ -421,14 +489,15 @@
                     raise Exception(
                         f"Link {linkpath} exists, but it doesn't point to the right place in the cache ({new_path}). "
                         f"The link currently points to {realpath}. "
                         f"Output directory may have been created inadvertantly outside Makex. "
                         f" Delete or change this link."
                     )
         else:
+            # linkpath doesn't exist.
             if linkpath.is_symlink():
                 # we have a broken symlink
                 if fix:
                     # fix broken links automatically
                     realpath = linkpath.readlink().absolute()
                     logging.debug(
                         "Fixing broken link from %s to %s. Unlinking %s",
@@ -447,97 +516,103 @@
             #        target,
             #    )
 
             if not linkpath.parent.exists():
                 logging.debug("Creating parent of linked output directory: %s", linkpath.parent)
                 linkpath.parent.mkdir(parents=True)
 
-            logging.debug(
-                "Symlink %s[%s,symlink=%s] <- %s[%s,symlink=%s]",
-                new_path,
-                new_path.exists(),
-                new_path.is_symlink(),
-                linkpath,
-                linkpath.exists(),
-                linkpath.is_symlink()
-            )
             linkpath.symlink_to(new_path, target_is_directory=True)
 
-    def _evaluate_target(self, target: TargetObject, destroy_output=False) -> EvaluatedTarget:
+    def _get_output_file_status(self, path: Path) -> FileStatus:
+        checksum = None
+        if path.exists():
+            checksum = self._checksum_file(path)
+        status = FileStatus(path, checksum=checksum)
+        return status
+
+    def _evaluate_target(self,
+                         target: TargetObject,
+                         destroy_output=False) -> tuple[EvaluatedTarget, list[Exception]]:
         # transform the target object into an evaluated object
         # check the inputs of target are available
         seen = set()
         target_input_path = target.path_input()
         target_output_path = None
         ctx = self.ctx
         #trace("Input path set to %s", target_input_path)
         inputs = []
         requires: list[EvaluatedTarget] = []
+        errors = []
 
         # We may have any number of objects passed in target(requires=[]).
         # Translate them for the EvaluatedTarget.
         # XXX: there's some duplication here with _iterate_makefile_requirements
         # XXX: most of this should be duck-typed with a _evaluate() method on the Element. However,
         #  since nodes are part of the makex file scripting api, we can't just expose hidden methods on objects.
         for node in target.requires:
             #trace("Process requirement %r", node)
             if isinstance(node, PathElement):
                 path = resolve_path_element_workspace(
                     ctx, target.workspace, node, target_input_path
                 )
 
                 if not path.exists():
-                    inputs.append(
-                        FileStatus(
-                            path=path,
-                            error=ExecutionError(
-                                "Missing input file: {node}", target, node.location
-                            ),
-                        )
-                    )
+                    error = ExecutionError("Missing input file: {node}", target, node.location)
+                    errors.append(error)
+
+                    inputs.append(FileStatus(path=path, error=error))
                 else:
-                    if not path.is_dir():
-                        # checksum the input file if it hasn't been
-                        checksum = self._checksum_file(path)
-                        seen.add(path)
-                        inputs.append(FileStatus(
-                            path=path,
-                            checksum=checksum,
-                        ))
-            elif isinstance(node, Glob):
-                for path in resolve_glob(
-                    ctx, target, target_input_path, node, {ctx.output_folder_name}
-                ):
+                    if path.is_dir():
+                        continue
+
+                    # checksum the input file if it hasn't been
                     checksum = self._checksum_file(path)
                     seen.add(path)
                     inputs.append(FileStatus(
                         path=path,
                         checksum=checksum,
                     ))
+            elif isinstance(node, Glob):
+                try:
+                    for path in resolve_glob(
+                        ctx, target, target_input_path, node, {ctx.output_folder_name}
+                    ):
+                        checksum = self._checksum_file(path)
+                        seen.add(path)
+                        inputs.append(FileStatus(
+                            path=path,
+                            checksum=checksum,
+                        ))
+                except FileNotFoundError as e:
+                    raise PythonScriptError(f"Error finding files: {e}", node.location)
+
             elif isinstance(node, FindFiles):
                 # find(path, pattern, type=file|symlink)
                 if node.path:
                     path = resolve_path_element_workspace(
                         ctx, target.workspace, node.path, target_input_path
                     )
                 else:
                     path = target_input_path
 
                 # TODO: optimize find
                 i = 0
 
                 debug("Searching for files %s: %s", path, node.pattern)
-                for i, file in enumerate(resolve_find_files(ctx, target, path, node.pattern, ignore_names={ctx.output_folder_name})):
-                    trace("Checksumming input file %s", file)
-                    checksum = self._checksum_file(file)
-                    seen.add(file)
-                    inputs.append(FileStatus(
-                        path=file,
-                        checksum=checksum,
-                    ))
+                try:
+                    for i, file in enumerate(resolve_find_files(ctx, target, path, node.pattern, ignore_names={ctx.output_folder_name})):
+                        #trace("Checksumming input file %s", file)
+                        checksum = self._checksum_file(file)
+                        seen.add(file)
+                        inputs.append(FileStatus(
+                            path=file,
+                            checksum=checksum,
+                        ))
+                except FileNotFoundError as e:
+                    raise PythonScriptError(f"Error finding files: {e}", node.location)
 
                 if i:
                     debug("Found %s files in %s", i, path)
             elif isinstance(node, StringValue):
                 # XXX: This shouldn't happen. StringValues should already be transformed.
                 raise NotImplementedError(f"Got {type(node)}: {node}")
             elif isinstance(node, TargetObject):
@@ -546,21 +621,15 @@
                 requires.append(requirement)
             elif isinstance(node, TargetReferenceElement):
                 # XXX: reference to an external target
                 # translate the target reference and resolve it
                 name = node.name
                 # resolve the target reference
                 path = node.path
-                #debug(
-                #    "Evaluate reference %s: %s: %r %s",
-                #    name,
-                #    path,
-                #    path,
-                #    node.location if path else None
-                #)
+                #debug("Evaluate reference %s: %s: %r %s", name, path, path, node.location if path else None)
                 if path is None:
                     # we have a local reference
                     _path = Path(target.makex_file_path)
                     ref = ResolvedTargetReference(name, _path, location=node.location)
                 elif isinstance(path, StringValue):
                     _path = resolve_string_path_workspace(
                         ctx, target.workspace, path, target_input_path
@@ -576,15 +645,15 @@
                             path.location
                         )
                         #stop_and_error(error)
                         raise error
 
                     ref = ResolvedTargetReference(name, makex_file, location=path.location)
                 elif isinstance(path, PathObject):
-                    # XXX: odd case of referring to a build_path in a target referene
+                    # XXX: odd case of referring to a build_path in a target reference
                     raise NotImplementedError("")
                 elif isinstance(path, PathElement):
                     _path = resolve_path_element_workspace(
                         ctx, target.workspace, path, target_input_path
                     )
 
                     # find the makex file inside of path
@@ -617,69 +686,48 @@
                     f"Invalid requirement in target {target.key()} {type(node)}",
                     target,
                     target.location
                 )
 
         outputs: list[FileStatus] = []
 
-        unnamed_outputs = []
-        output_dict: dict[Union[str, None], list[FileStatus]] = {None: unnamed_outputs}
+        unnamed_outputs: list[FileStatus] = []
+        output_dict: dict[Union[int, str, None], Union[FileStatus, list[FileStatus]]] = {
+            None: unnamed_outputs
+        }
 
         # only create if we have runs (or somehow, just outputs)
         target_output_path, cache_path = resolve_target_output_path(ctx, target=target)
 
         if target.outputs:
             #debug("Rewrite output path %r %r %s", target_output_path, target.path, target)
+            # TODO: use a method on TargetObject to get/transform outputs
+            for k, path_like in target.outputs_dict.items():
 
-            def _get_output_file_status(path: Path) -> FileStatus:
-                checksum = None
-                if path.exists():
-                    checksum = self._checksum_file(path)
-                status = FileStatus(path, checksum=checksum)
-                return status
-
-            # TODO: this method should be moved to the makex file module. _resolve_pathlike() fits the bill.
-            def _transform_output_to_path(
-                base: Path, value: Union[StringValue, PathElement, PathObject]
-            ) -> Path:
-                # TODO: we probably won't get any StringValues as they are transformed earlier
-                if isinstance(value, StringValue):
-                    path = resolve_string_path_workspace(ctx, target.workspace, value, base)
-                elif isinstance(value, PathElement):
-                    # TODO: we should use the resolved path here
-                    path = resolve_path_element_workspace(ctx, target.workspace, value, base)
-                elif isinstance(value, PathObject):
-                    return value.path
-                else:
-                    raise NotImplementedError(f"Invalid output type {type(value)}: {value!r}")
-
-                return path
-
-            if target.outputs_dict: # TODO: no branch needed here
-                for k, v in target.outputs_dict.items():
-
-                    for value in v:
-                        if False:
-                            path = _resolve_pathlike(
-                                ctx,
-                                target,
-                                target_output_path,
-                                "outputs",
-                                value=value,
-                                error_string="Invalid output type {type(value)}: {value!r}",
-                            )
-                        path = _transform_output_to_path(target_output_path, value)
+                if isinstance(path_like, list):
+                    for value in path_like:
+                        path = _transform_output_to_path(ctx, target, target_output_path, value)
                         trace("Check target output: %s", path)
-                        status = _get_output_file_status(path)
+                        status = self._get_output_file_status(path)
                         if k is None:
                             unnamed_outputs.append(status)
                         else:
                             output_dict.setdefault(k, []).append(status)
 
                         outputs.append(status)
+                else:
+                    path = _transform_output_to_path(ctx, target, target_output_path, path_like)
+                    trace("Check target output: %s", path)
+                    status = self._get_output_file_status(path)
+                    if k is None:
+                        unnamed_outputs.append(status)
+                    else:
+                        output_dict[k] = status
+
+                    outputs.append(status)
 
         # TODO: search for any input files from the last run missing in this one
         if False:
             for file in self._get_last_input_files(target):
                 if file not in seen:
                     #errors.append()
                     inputs.append(
@@ -687,125 +735,141 @@
                             path=path,
                             error=ExecutionError("Missing input file: {node}", target),
                         )
                     )
                     #errors.append()
 
         #debug("Pre-eval requires %s", requires)
-        # Create a Evaluated target early, which we can pass to Runnables so they can easily create arguments (below).
-        # XXX:
-        runnables = []
+        # Create a Evaluated target early, which we can pass to Actions so they can easily create arguments (below).
+        actions: list[InternalAction] = []
         evaluated = EvaluatedTarget(
             name=target.name,
             path=target_output_path,
             input_path=target_input_path,
             inputs=inputs,
             outputs=outputs,
+            output_dict=output_dict,
             # TODO: append these commands in a separate thread
-            runnables=runnables,
+            actions=actions,
             # use the existing requires list for performance
             # we don't need to copy/recreate here because they key/serialize the same
             requires=requires,
             location=target.location,
             cache_path=cache_path,
             makex_file=target.makex_file,
             workspace=target.workspace,
         )
 
         # TODO: queue target transformation in a separate pool and return a future here (once evaluated)
-        # TODO:
-
-        def figure_out_location(obj, default):
-            location = getattr(obj, "location", None)
-
-            if location and isinstance(location, FileLocation):
-                return location
-            else:
-                location = None
-
-            if location is None: # or isinstance(obj, FileLocation) is False:
-                return default
-
-            return location
 
         if target.commands is not None and isinstance(target.commands, ListTypes) is False:
             location = figure_out_location(target.commands, target.location)
             err = PythonScriptError(
-                f"Target runs argument must be a list. Got {target.commands!r}", location
+                f"Target actions argument must be a list. Got {target.commands!r}", location
             )
             raise err
 
         for command in target.commands:
-            # TODO: check we actually got a runnable
-
-            if isinstance(command, InternalRunnableBase) is False:
-                error("Got %s", type(command))
-
+            # TODO: check we actually got a Action
+            if isinstance(command, ListTypes):
+                for c in command:
+                    if isinstance(c, InternalActionBase) is False:
+                        location = figure_out_location(c, target.location)
+
+                        err = PythonScriptError(
+                            f"Invalid action in target {target}: {c!r}",
+                            location,
+                        )
+                        raise err
+                    else:
+                        arguments = c.transform_arguments(ctx, evaluated)
+                        actions.append(InternalAction(c, arguments))
+            elif isinstance(command, InternalActionBase) is False:
                 location = figure_out_location(command, target.location)
 
                 err = PythonScriptError(
-                    f"Invalid runnable in target {target}: {command!r}",
+                    f"Invalid action in target {target}: {command!r}",
                     location,
                 )
                 raise err
+            else:
+                arguments = command.transform_arguments(ctx, evaluated)
+                actions.append(InternalAction(command, arguments))
 
-            arguments = command.transform_arguments(ctx, evaluated)
-            runnables.append(InternalRunnable(command, arguments))
-
-        return evaluated
+        return evaluated, errors
 
     def _memory_has_target(self, hash: str):
         return hash in self._target_hash
 
-    def _check_target_dirty(self, evaluated: EvaluatedTarget) -> tuple[bool, list[Exception]]:
+    def _check_target_dirty(
+        self,
+        evaluated: EvaluatedTarget,
+        h=None,
+    ) -> tuple[bool, list[Exception]]:
+
+        h = h or self._get_target_hash(evaluated)
+        target_key = evaluated.key()
+
+        trace(f"Target hash is: %s of %r (exists=%s)", h, target_key, h in self._target_hash)
+
+        if target_key in self._executed_keys:
+            # we just executed this target, report it as dirty.
+            # TODO: determine if this is correct.
+            trace(f"Target is dirty because it was just executed in this process. (%s)", target_key)
+            return True, []
+
+        # TODO: we need to cache dirty checking so this doesn't go too deep.
+        for require in evaluated.requires:
+            dirty, _ = self._check_target_dirty(require)
+            if dirty:
+                trace("Requirement of %s is dirty: %s", evaluated.key(), require.key())
+                return True, []
 
         # XXX: Targets without any outputs are always dirty. We can't compare the outputs.
         if len(evaluated.outputs) == 0:
-            trace(f"Target is dirty because it has no outputs. (%s)", evaluated.key())
+            trace(f"Target is dirty because it has no declared outputs. (%s)", target_key)
             return True, []
 
         # XXX: Targets with outputs, but without any input files or requirements are always dirty.
         if len(evaluated.inputs) == 0 and len(evaluated.requires) == 0:
-            trace(
-                f"Target is dirty because it has no requirements or inputs. (%s)", evaluated.key()
-            )
+            trace(f"Target is dirty because it has no requirements or inputs. (%s)", target_key)
             return True, []
 
-        h = self._get_target_hash(evaluated)
-        trace(f"Target hash is: %s of %r (exists=%s)", h, evaluated.key(), h in self._target_hash)
         # First, Check the in-memory cache
         target_dirty = self._memory_has_target(h) is False
 
         errors = []
 
+        _outputs_checked = False
         # Next, Check if the [shared] disk cache has the target
         if DATABASE_ENABLED:
             if True: # only check if the in memory is empty
-                db_has_target = self._disk_metadata.has_target(h)
+                db_has_target = self._disk_metadata.has_target(target_key, h)
 
                 # We need to verify the outputs here because it's possible they are missing/screwed up, and we were not the ones who produced the target.
                 if db_has_target is True:
                     debug(
                         f"Target in database. Checking outputs... (%r, hash=%r).",
                         evaluated.key(),
                         h
                     )
-                    if self._check_outputs_stale_or_missing(evaluated):
+
+                    if self._check_outputs_stale_or_missing(evaluated, h):
                         # db has a target produced with the specified hash. outputs are still valid.
-                        debug(
-                            f"Target is dirty because the outputs are stale (%r).", evaluated.key()
-                        )
+                        debug(f"Target is dirty because the outputs are stale (%r).", target_key)
                         target_dirty = True
                     else:
-                        debug(f"Outputs of target are not stale (%r, hash=%r).", evaluated.key(), h)
+                        debug(f"Outputs of target are not stale (%r, hash=%r).", target_key, h)
                         target_dirty = False
+
+                    _outputs_checked = True
                 else:
                     debug(
                         f"Target is dirty because the database doesn't have the target (%r, hash=%r).",
-                        evaluated.key(),
+                        target_key,
                         h
                     )
                     target_dirty = True
 
                 if target_dirty is True:
                     return target_dirty, errors
 
@@ -813,15 +877,15 @@
             # memory or db has the target
             #debug(f"Skipping target. Not dirty. (%r, hash=%r).", evaluated.key(), h)
             return target_dirty, errors
         else:
             # neither have the target
             debug(
                 "Target is dirty because hash isn't in memory or database: (%r, hash=%r)",
-                evaluated.key(),
+                target_key,
                 h,
             )
 
         if False:
             #hash = evaluated.hash(self.ctx)
 
             # targets with requires are not dirty by default.
@@ -841,48 +905,36 @@
 
                 trace(f"Checksum checked for {input.path}: {input.checksum} (dirty={target_dirty})")
                 #checksums.append(target_dirty)
             else:
                 # targets without any inputs are always dirty.
                 target_dirty = True
 
-        if target_dirty is False:
-            # check for any missing outputs
-            for output in evaluated.outputs:
-                path = Path(output.path)
-                trace(f"Check output %s: %s", path, path.exists())
-                if not path.exists():
-                    warning(f"missing output file {output.path}. dirty.")
-                    target_dirty = True
-            # TODO: check if the outputs target hash is different
+        if _outputs_checked is False and target_dirty is False:
+            # check for any missing outputs...
+            target_dirty = self._check_outputs_stale_or_missing(evaluated, None)
 
         return target_dirty, errors
 
     def _remove_from_queue(self, target):
         try:
             self.queued.remove(target.key())
         except ValueError as e:
             error("Can't find %s in %s %r", target.key(), self.queued, target)
             raise e from e
 
-    def _mark_target_complete(self, target: EvaluatedTarget, queued=True):
-        # queued may be false if we mark it complete before running it
-        if queued:
-            try:
-                self.queued.remove(target.key())
-            except ValueError as e:
-                error("Can't find %s in %s %r", target.key(), self.queued, target)
-                raise e from e
-
+    def _mark_target_complete(self, target: EvaluatedTarget):
+        # Mark a target as complete. This is called when the target is not dirty.
         self._target_status[target.key()] = True
 
     def _mark_target_executed(self, target: EvaluatedTarget):
         # Mark the target as actually executed; like, a thread was created to run it.
         if target not in self.finished:
             self.finished.append(target)
+            self._executed_keys.add(target.key())
 
         try:
             self.queued.remove(target.key())
         except ValueError as e:
             error("Can't find %s in %s %r", target.key(), self.queued, target)
             raise e from e
 
@@ -893,34 +945,47 @@
         target: TargetObject,
     ) -> tuple[Optional[EvaluatedTarget], Optional[list[Exception]]]:
 
         # Don't execute any more if we have a stop flag.
         if self.stop.is_set():
             return None, None
 
-        # XXX: Make sure any targets that need to be written are. Otherwise, the Target might not be stored because
-        #  of a long running Target/process (e.g. a development server target) we're just about to execute.
+        # XXX: Make sure any targets that need to be written are.
+        #  Otherwise, the Target mights not be cached/stored properly because of a long running Target/process
+        #  (e.g. a development server target) we're just about to execute that doesn't terminate properly.
+
+        # TODO: handle the database problem and endless targets better
+        #if target.endless:
         self._write_queued_to_database()
 
         if target.path:
             if target.path.resolved:
+                # XXX: a fully resolved path was passed to the target output
+                #  Don't delete because it could be somewhere on the users filesystem which they don't expect to be deleted.
+                # TODO: we should remove this branch once we remove use of Target.path
                 delete_output = False
+            else:
+                delete_output = True
         else:
             delete_output = True
 
         debug(f"Begin evaluate target {target}...")
         # queue the requirements for execution if all dependencies are completed
         try:
-            evaluated: EvaluatedTarget = self._evaluate_target(target)
+            evaluated, errors = self._evaluate_target(target)
+
+            if errors:
+                raise MultipleErrors(errors)
         except (PythonScriptError, ExecutionError) as e:
             #logging.exception(e)
             #self.errors.append(e)
             # XXX: target evaluation errors must stop all execution.
             #self.stop.set()
             return None, [e]
+
         # TODO: have a future here; once complete, then enable the actual execution. evaluations may come out of order,
         #  so, we have to synchronize the evaluation order with the intended execution order
         """
         
         queue = [a, b, c, d]  # required order of execution, as planned
         
         # put a, b, c and d on evaluation queue/pool (threads=2).
@@ -931,15 +996,15 @@
         # ...
         
         # c evaluates early, needs d. d is still in eval list.
         eval_list = [a, b, d]
         execute_wait_list = [c]
         execute_list = []
         
-        # d evauluates early, add to wait
+        # d evaluates early, add to wait
         eval_list = [a, b]
         execute_wait_list = [c,d]
         execute_list = []
         
         # move d to execute because it has no deps
         eval_list = [a, b]
         execute_wait_list = [c]
@@ -967,15 +1032,15 @@
         execute_list = [d, c, b]
         
         # execute a because all of it is on execute list
         eval_list = []
         execute_wait_list = []
         execute_list = [d, c, b, a]
         
-        Execute list is ordered correctly, but it is not topographic, parallelized.
+        Execute list is ordered correctly, but it is not topographic/parallelized.
         The execute_list/queue is processed similarly; waiting for target dependants to finish before starting the target.
         """
 
         #self.ctx.ui.print(f"Evaluated target: {target.key()}")
         debug("Evaluated target: %s", evaluated.key())
 
         self.graph_2.add_target(evaluated)
@@ -983,110 +1048,130 @@
         target_dirty, errors = self._check_target_dirty(evaluated)
 
         # all([]) -> True
         #target_dirty = all(checksums)
 
         if self.analysis_mode is True:
             # XXX: make sure to mark complete so we don't hang.
-            self._mark_target_complete(evaluated, queued=False)
+            self._mark_target_complete(evaluated)
             return evaluated, errors
 
         if errors:
             # STOP NOW, Raise errors
             raise MultipleErrors(errors)
 
         if self.force:
             # force the execution
-            self._queue_target_on_pool(evaluated, delete_output)
+            self._queue_target_on_pool(evaluated, delete_output, hash)
             return evaluated, None
 
         # dirty checking applicable
         if target_dirty is False:
-            self._mark_target_complete(evaluated, queued=False)
-            #key = target.key()
-            #if key in self.queued:
-            #    self.queued.remove(key)
+            self._mark_target_complete(evaluated)
+            #self._queue_for_database(evaluated)
             debug("Skipping target. Not dirty: %s", evaluated.key())
             return evaluated, None
 
         info("Target has been deemed dirty. Queueing for execution: %s", evaluated.key())
-        self._queue_target_on_pool(evaluated, delete_output)
+        self._queue_target_on_pool(evaluated, delete_output, hash)
         return evaluated, None
 
-    def _queue_target_on_pool(self, evaluated: EvaluatedTarget, delete_output) -> None:
+    def _queue_target_on_pool(self, evaluated: EvaluatedTarget, delete_output, hash) -> None:
         # TODO: we should get a future here.
         #  if there was an exception, stop everything, both execution and evaluation.
         #  if all the requirements have evaluated (or no requirements), execute.
         #  if not, add to execute wait queue.
         #  process execute wait queue each for each call. check if target all of each targets deps have finished evaluation
         #   if all of the deps have evaluated, push onto execute queue
         #   if none or only some of the deps have evaluated, keep it waiting
         #info(f"Queue target for execution {evaluated}")
 
-        if delete_output and evaluated.cache_path.exists():
-            if REMOVE_CACHE_DIRTY_TARGETS_ENABLED:
+        cache_exists = evaluated.cache_path.exists()
+        if cache_exists:
+            if REMOVE_CACHE_DIRTY_TARGETS_ENABLED and delete_output:
                 debug(
                     "Removing cache of %s (%s) because target is dirty.",
                     evaluated.key(),
                     evaluated.cache_path
                 )
                 # remove the cache if the target is dirty
                 rmtree(evaluated.cache_path)
+                evaluated.cache_path.unlink(missing_ok=True)
 
+                logging.debug("Creating output directory %s", evaluated.cache_path)
+                evaluated.cache_path.mkdir(parents=True, exist_ok=True)
         # create a single link from _output_ to cache's _output_
-        if not evaluated.cache_path.exists():
+        elif cache_exists is False:
             logging.debug("Creating output directory %s", evaluated.cache_path)
             evaluated.cache_path.mkdir(parents=True, exist_ok=True)
 
+        debug("Output2 %s", list(evaluated.input_path.iterdir()))
         # autogenerated path
         if SYMLINK_PER_TARGET_ENABLED is False:
             # create link Target.input_path / _output_ -> Target.cache_path.parent (_output_)
             self._create_output_link(evaluated, evaluated.cache_path.parent)
         else:
             # create a link from Target.input_path / _output_ / Target.id - > Target.cache_path
             raise NotImplementedError()
 
         self.queued.append(evaluated.key())
-        future = self.pool.submit(self._execute_target_thread, self.ctx, evaluated)
-        future.add_done_callback(lambda future, x=evaluated: self.target_completed(x, future))
+        future = self.pool.submit(self._execute_target_thread, self.ctx, evaluated, hash)
+        future.add_done_callback(lambda future, x=evaluated: self._target_completed(x, future))
         return None
 
     def _get_last_input_files(self, target: EvaluatedTarget) -> list[Path]:
         metadata = self._load_target_metadata(target)
         if metadata is None:
             return []
         return metadata.inputs
 
-    def _check_outputs_stale_or_missing(self, target):
+    def _check_output_hash_valid(self, path: Path, hash: str):
+        # check the hash stored in the output file matches our target
+        if hash != _get_xattr(path, _XATTR_OUTPUT_TARGET_HASH).decode("ascii"):
+            trace("Target.hash != output.hash: %s %s", path, hash)
+            return False
+
+        return True
+
+    def _check_outputs_stale_or_missing(self, target: EvaluatedTarget, target_hash: str):
         # Return True if any outputs are missing or stale
         dirty = True
         for output in target.outputs:
             path = output.path
             if path.exists():
                 # TODO: do a checksum of the output and compare
                 checksum = self._checksum_file(path)
 
                 if self._is_checksum_stale(path, checksum):
                     trace("Checksum of %s is stale: %s", path, checksum)
                     # checksum is not stale
                     dirty = True
                     break
+
+                # TODO: check if the outputs target hash is different
+                if STORE_TASK_HASH_IN_OUTPUT_FILES and self._check_output_hash_valid(
+                    path, target_hash
+                ) is False:
+                    dirty = True
+                    break
             else:
                 # missing output
                 dirty = True
                 break
         else: # no break; has no outputs, or all checksums/files exist.
             dirty = False
 
         return dirty
 
-    def get_target_output_errors(self, target: EvaluatedTarget) -> list[Exception]:
+    def _get_target_output_errors(self, target: EvaluatedTarget) -> list[Exception]:
         # Check outputs are produced after target execution.
         # return errors if they aren't, or if something else is wrong.
         if self.ctx.dry_run:
+            # Dry runs can't have any errors because they didn't do anything.
+            # TODO: check if this is right.
             return []
 
         errors = []
         for output in target.outputs:
             path = output.path
             if not path.exists():
                 errors.append(
@@ -1106,15 +1191,15 @@
 
         return hash
 
     def _put_target_hash(self, target: EvaluatedTarget, hash):
         trace("Store target hash %s %s", target.key(), hash)
         self._target_hash[target.key()] = hash
 
-    def target_completed(self, target: EvaluatedTarget, result: Future[TargetResult]):
+    def _target_completed(self, target: EvaluatedTarget, result: Future[TargetResult]):
         # Called after the Future is completed.
         # Called in *this* thread (not the thread in which the target was executed).
         assert isinstance(target, EvaluatedTarget)
 
         self._mark_target_executed(target)
 
         debug("Target complete %s", target)
@@ -1126,32 +1211,26 @@
         exc = result.exception()
         if exc:
             if self.ctx.debug or isinstance(exc, (ExecutionError, PythonScriptError)) is False:
                 # also show it here on debug mode because it'll get swallowed
                 # log unknown/unprintable
                 logging.exception(exc)
                 pass
-            #error("@@@@@@@@ERROR RUNNING TARGET: %s", result.exception())
-            #traceback.print_exception(target.exception())
+            #error("ERROR RUNNING TARGET: %s", result.exception())
             self.errors.append(exc)
             self.stop.set()
-            return
-
-        has_error = False
+            return None
 
         if True:
-            errors = self.get_target_output_errors(target)
+            errors = self._get_target_output_errors(target)
 
             if errors:
                 self.errors += errors
                 #self.stop.set()
-                has_error = True
-
-        if has_error:
-            return
+                return None
 
         # XXX: Store in database as soon as we're done with a success. No later.
         self._queue_for_database(target)
 
     def _queue_for_database(self, target: EvaluatedTarget):
         if self.ctx.dry_run is True:
             return None
@@ -1163,59 +1242,64 @@
             return None
 
         while self._database_queue:
             target = self._database_queue.popleft()
             trace("Writing queue target %r to database", target.key())
             self._store_database(target)
 
-    def _execute_target_thread(self, ctx: Context, target: EvaluatedTarget):
+    def _write_target_hash_to_outputs(self, target_hash: bytes, outputs: list[FileStatus]):
+        #target_hash_bytes = target_hash.encode("utf-8")
+        for output in outputs:
+            _set_xattr(output.path, _XATTR_OUTPUT_TARGET_HASH, target_hash)
 
-        # this is run in a separate thread
+    def _execute_target_thread(self, ctx: Context, target: EvaluatedTarget, target_hash):
+        # this is run in a separate thread...
         debug(f"Begin execution of target: {target} [thread={threading.current_thread().ident}]")
 
         ctx.ui.print(f"Execute target: {target.key()}")
         output = StringIO()
 
         # create a copy of the ctx.environment, so we can set ctx.environment variables throughout the process.
         with ctx.new_environment() as subcontext:
             #context = ctx or subcontext
             context = subcontext
-            for command in target.runnables or []:
+            for command in target.actions or []:
                 debug(f"- Execute command (%s): %r", target.name, command)
 
                 if self.analysis_mode:
                     continue
 
-                if True:
-                    # XXX: right now we want errors from runnables to propagate outwards.
-                    #try:
-                    execution = command(context, target)
-
-                    if execution is None or execution.status is None:
-                        message = f"Runnable {command!r} did not return a valid output. Got {type(execution)}"
-                        raise ExecutionError(message, target, command.location or target.location)
-
-                    if execution.status != 0:
-                        # \n\n {execution.output} \n\n {execution.error}
-                        string = [
-                            f"Error running the runnable for target ",
-                            f"{brief_target_name(context, target, color=True)}:{target.location.line} (exit={execution.status}) \n",
-                            f"\tThe process had an error and returned non-zero status code ({execution.status}). See above for any error output."
-                        ]
-                        raise ExecutionError(
-                            "".join(string), target, command.location or target.location
-                        )
+                # XXX: right now we want errors from Actions to propagate outwards.
+                #try:
+                execution = command(context, target)
+
+                if execution is None or execution.status is None:
+                    message = f"Action {command!r} did not return a valid output. Got {type(execution)}"
+                    raise ExecutionError(message, target, command.location or target.location)
+
+                trace("Execution return status: %s", execution)
+
+                if execution.status != 0: #not in {0, CORRECTED_RETURN_CODE}:
+                    # \n\n {execution.output} \n\n {execution.error}
+                    string = [
+                        f"Error running the action for target ",
+                        f"{brief_target_name(context, target, color=True)}:{target.location.line} (exit={execution.status}) \n",
+                        f"\tThe process had an error and returned non-zero status code ({execution.status}). See above for any error output."
+                    ]
+                    raise ExecutionError(
+                        "".join(string), target, command.location or target.location
+                    )
 
-                    if execution.output:
-                        # XXX: not required as execution dumps stdout. we may want to capture
-                        output.write(execution.output)
-
-                    #except Exception as e:
-                    #    logging.exception(e)
-                    #   pass
+                if execution.output:
+                    # XXX: not required as execution dumps stdout. we may want to capture
+                    output.write(execution.output)
+
+                #except Exception as e:
+                #    logging.exception(e)
+                #   pass
 
         debug(f"Finished execution of target: {target}")
 
-        return TargetResult(target, output=output.getvalue())
+        if STORE_TASK_HASH_IN_OUTPUT_FILES:
+            self._write_target_hash_to_outputs(target_hash, target.outputs)
 
-    def execution_completed(self):
-        debug("completed!")
+        return TargetResult(target, output=output.getvalue())
```

### Comparing `makex-20240203/python/makex/executor_test.py` & `makex-20240401/python/makex/executor_test.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,25 @@
 from pathlib import Path
 from typing import (
     Any,
     Union,
 )
 
 import pytest
-
 from makex.context import Context
 from makex.executor import Executor
-from makex.make_file import (
-    InternalRunnableBase,
+from makex.makex_file import (
+    InternalActionBase,
+    MakexFile,
+    TargetObject,
+)
+from makex.makex_file_parser import TargetGraph
+from makex.makex_file_types import (
     PathElement,
     ResolvedTargetReference,
-    TargetGraph,
-    TargetObject,
     TargetReferenceElement,
 )
 from makex.protocols import (
     CommandOutput,
     StringHashFunction,
 )
 from makex.python_script import FileLocation
@@ -62,18 +64,19 @@
     ctx.workspace_object = Workspace(tmp_path)
 
     pathmaker = PathMaker()
     path = pathmaker.path
 
     l = fake_location(tmp_path / "Makexfile")
 
-    d = TargetObject("d", location=l)
-    b = TargetObject("b", requires=[d], location=l)
-    c = TargetObject("c", requires=[d], location=l)
-    a = TargetObject("a", requires=[b, c], location=l)
+    makex_file = MakexFile(None, tmp_path / "Makexfile")
+    d = TargetObject("d", makex_file=makex_file, location=l)
+    b = TargetObject("b", requires=[d], makex_file=makex_file, location=l)
+    c = TargetObject("c", requires=[d], makex_file=makex_file, location=l)
+    a = TargetObject("a", requires=[b, c], makex_file=makex_file, location=l)
     #errors = e.execute_targets(a)
 
     g = TargetGraph()
     g.add_targets(ctx, a, b, c, d)
     print(list(g.topological_sort_grouped([a])))
     assert True
 
@@ -133,15 +136,15 @@
     #    path = parent / path
     #else:
     #    path = parent / path
 
     return PathElement(*args, resolved=None)
 
 
-class WriteTestRunnable(InternalRunnableBase):
+class WriteTestAction(InternalActionBase):
     def __init__(self, path: str, text, location=None):
         self.path: str = path
         self.text = text
         self.location = location
 
     def __repr__(self):
         return f"Write({self.path}) -> {self.text}"
@@ -165,15 +168,15 @@
         logging.debug("Writing file at %s", path)
         path.write_text(self.text)
 
         return CommandOutput(0)
 
 
 def write(path: str, text=None):
-    return WriteTestRunnable(path, text or str(path))
+    return WriteTestAction(path, text or str(path))
 
 
 def fake_location(path):
     return FileLocation(0, 0, path)
 
 
 def test_input_ouput(tmp_path: Path):
@@ -206,45 +209,51 @@
     o_pathmaker = PathMaker(output)
     opath = o_pathmaker.path
 
     i_pathmaker = PathMaker(input)
     ipath = i_pathmaker.path
 
     debug("$SSSSS %s", opath())
+
+    makex_file = MakexFile(None, input_make_file)
     d = TargetObject(
         "d",
         path=opath(),
         requires=[ipath("d")],
         outputs=[opath("d")],
         run=[write("d")],
         location=location,
+        makex_file=makex_file,
     )
     b = TargetObject(
         "b",
         path=opath(),
         requires=[ipath("b"), d],
         outputs=[opath("b")],
         run=[write("b")],
         location=location,
+        makex_file=makex_file,
     )
     c = TargetObject(
         "c",
         path=opath(),
         requires=[ipath("c"), d],
         outputs=[opath("c")],
         run=[write("c")],
         location=location,
+        makex_file=makex_file,
     )
     a = TargetObject(
         "a",
         path=opath(),
         requires=[ipath("a"), b, c],
         outputs=[opath("d")],
         run=[write("a")],
         location=location,
+        makex_file=makex_file,
     )
 
     ctx = Context()
     ctx.workspace_object = Workspace(tmp_path)
     ctx.graph = g = TargetGraph()
     g.add_targets(ctx, a, b, c, d)
```

### Comparing `makex-20240203/python/makex/file_checksum.py` & `makex-20240401/python/makex/file_checksum.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,35 +12,44 @@
     Tuple,
 )
 
 # True to use builtin python xattr functions instead of xattr pypi package
 BUILTIN_XATTR = True
 
 if BUILTIN_XATTR:
+    from os import (
+        getxattr,
+        removexattr,
+        setxattr,
+    )
 
     def get_xattr(path, attribute):
-        return os.getxattr(path, attribute)
+        return getxattr(path, attribute)
 
     def set_xattr(path, attribute, value):
-        return os.setxattr(path, attribute, value)
+        return setxattr(path, attribute, value)
 
     def remove_xattr(path, attribute):
-        return os.removexattr(path, attribute)
+        return removexattr(path, attribute)
 
 else:
-    import xattr
+    from xattr import (
+        getxattr,
+        removexattr,
+        setxattr,
+    )
 
     def get_xattr(path, attribute):
-        return xattr.getxattr(path, attribute)
+        return getxattr(path, attribute)
 
     def set_xattr(path, attribute, value):
-        return xattr.setxattr(path, attribute, value=value)
+        return setxattr(path, attribute, value=value)
 
     def remove_xattr(path, attribute):
-        return xattr.removexattr(path, attribute)
+        return removexattr(path, attribute)
 
 
 INODE_IN_FINGERPRINT = False
 
 # must be prefixed with user. otherwise we will get OSError, Operation not supported
 TEST_KEY = b"user.test"
 TEST_VALUE = b"test"
@@ -70,18 +79,14 @@
     """
     Calculates the digest/checksum of a file, and stores it in extended attributes.
 
     In order to maintain stability, if any of the following change, the checksum is recomputed.
 
     mtime
     size
-    inode number
-    file mode
-    owner uid and gid
-    (targets only) the sequence number of the last time it was built
 
     We use mtime because ctime is too sensitive/false positive.
 
     """
     class Type(Enum):
         SHA256 = "sha256"
         MD5 = "md5"
@@ -99,14 +104,20 @@
             return f"{self.type.value}:{self.value}:{self.fingerprint}"
 
         return f"{self.type.value}:{self.value}"
 
     def __hash__(self):
         return hash(f"{self.type.value}:{self.value}")
 
+    def write(self, path: Path):
+        type = self.type
+        csum = self.value
+        fingerprint = self.fingerprint
+        set_xattr(path, f"user.checksum.{type.value}", bytes(f"{csum}:{fingerprint}", "ascii"))
+
     @classmethod
     def parse(cls, string, fingerprint=None) -> "FileChecksum":
         assert isinstance(string, str)
         parts = string.split(":")
         if len(parts) == 2:
             type, value = parts
             return cls(FileChecksum.Type(type), value, fingerprint)
@@ -149,15 +160,20 @@
         # XXX: We should do this outside this function.
         if not os.access(path, os.W_OK):
             st = os.stat(path)
             new_mode = st.st_mode | stat.S_IXUSR | stat.S_IWGRP | stat.S_IWGRP | stat.S_IWRITE
             LOGGER.debug(f"Updating file mode {new_mode}: %s", path)
             os.chmod(path, new_mode)
 
-        set_xattr(path, f"user.checksum.{type.value}", bytes(f"{d}:{fingerprint}", "ascii"))
+        try:
+            set_xattr(path, f"user.checksum.{type.value}", bytes(f"{d}:{fingerprint}", "ascii"))
+        except OSError as e:
+            logging.error(e)
+            pass
+
         return cls(type, d, fingerprint)
 
     @classmethod
     def make(cls, path: Path, fingerprint: str, type: Type = Type.SHA256) -> "FileChecksum":
         d = get_digest(path)
         return cls(type, d, fingerprint)
 
@@ -277,17 +293,15 @@
             try:
                 fname = f.name.encode("utf-8")
                 set_xattr(fname, TEST_KEY, TEST_VALUE)
 
                 if get_xattr(fname, TEST_KEY) == TEST_VALUE:
                     remove_xattr(fname, TEST_KEY)
                     result = True
-            except IOError as e:
-
-                logging.error("IOERROR {}")
+            except (OSError,IOError) as e:
                 logging.exception(e)
                 result = False
 
         logging.debug("Check extended attributes supported at %s = %s.", path, result)
         # we shouldn't be here. faulty xattr implementation (can set, but not get).
         return result
 
@@ -304,15 +318,15 @@
             fingerprint = get_fingerprint(destination).encode("ascii")
 
         set_xattr(
             destination, f"user.checksum.{type.value}", bytes(f"{csum}:{fingerprint}", "ascii")
         )
 
     @staticmethod
-    def fingerprint(path: Path, type: Type = Type.SHA256):
+    def get_fingerprint(path: Path, type: Type = Type.SHA256) -> Optional[str]:
         return get_fingerprint(path)
 
 
 def copy_with_checksum(source, destination):
     shutil.copy2(source, destination)
     #shutil.copystat(source, destination)
     FileChecksum.copy(source, destination)
```

### Comparing `makex-20240203/python/makex/file_system.py` & `makex-20240401/python/makex/file_system.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,19 +13,19 @@
 )
 
 from makex.constants import BUILT_IN_REFLINKS
 
 REFLINKS_ENABLED = False
 
 if BUILT_IN_REFLINKS:
-    from makex.reflink import reflink
+    from makex.file_cloning import clone_file
     REFLINKS_ENABLED = True
 else:
     try:
-        from reflink import reflink
+        from file_cloning import clone_file
         REFLINKS_ENABLED = True
     except ImportError:
         REFLINKS_ENABLED = False
 
 
 def same_fs(file1, file2):
     dev1 = os.stat(file1).st_dev
@@ -104,15 +104,15 @@
     # IOError: [Errno 2] No such file or directory
     #a = os.stat(src)
     #b = os.stat(dest)
     #if a.st_ino == b.st_ino:
     #    return
 
     try:
-        reflink(src, dest)
+        clone_file(src, dest)
     except IOError as reflink_error:
         # Fall back to old [reliable] copy function if we get an EINVAL error.
         if reflink_error.errno == errno.EINVAL:
             logging.warning(
                 "Error with reflinks. Falling back to using copy.", exc_info=reflink_error
             )
             try:
```

### Comparing `makex-20240203/python/makex/flags.py` & `makex-20240401/python/makex/flags.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,16 +37,16 @@
 GLOBS_IN_OUTPUTS_ENABLED = _get_bool("GLOBS_IN_OUTPUTS_ENABLED", True)
 
 FIND_IN_INPUTS_ENABLED = _get_bool("FIND_IN_INPUTS_ENABLED", True)
 
 # Enable glob functions in the Target inputs list.
 GLOBS_IN_INPUTS_ENABLED = _get_bool("GLOBS_IN_INPUTS_ENABLED", True)
 
-# Enable globs in various arguments to runnables.
-GLOBS_IN_RUNNABLES_ENABLED = _get_bool("GLOBS_IN_RUNNABLES_ENABLED", DEVELOPMENT_ENABLED)
+# Enable globs in various arguments to Actions.
+GLOBS_IN_ACTIONS_ENABLED = _get_bool("GLOBS_IN_ACTIONS_ENABLED", DEVELOPMENT_ENABLED)
 
 # enable feature for variants of outputs
 VARIANTS_ENABLED = _get_bool("VARIANTS_ENABLED", False)
 
 # Enable the expand() function in makex files.
 EXPAND_FUNCTION_ENABLED = _get_bool("EXPAND_FUNCTION_ENABLED", False)
 
@@ -63,31 +63,42 @@
 # Inputs/outputs/Path element can all take absolute paths.
 ABSOLUTE_PATHS_ENABLED = _get_bool("ABSOLUTE_PATHS_ENABLED", True)
 
 # Enable/disable the shell() function.
 SHELL_FUNCTION_ENABLED = _get_bool("SHELL_FUNCTION_ENABLED", True)
 
 # Enable dictionaries/named outputs.
-NAMED_OUTPUTS_ENABLED = False
+NAMED_OUTPUTS_ENABLED = True
 
 # Enable embedding various paths in strings.
 # This should not be enabled until we carefully work in late string (joined or concatenated) evaluation
 # and early arugment processing.
 # Enable this in dev mode because we know what we want.
 # Disable for public because it can really footgun (cyclical deps).
 ENABLE_PATH_TO_STRING = _get_bool("ENABLE_PATH_TO_STRING", DEVELOPMENT_ENABLED)
 
+# Enable setting of target path.
+# We will likely set this to False by default.
+TARGET_PATH_ENABLED = _get_bool("TARGET_PATH_ENABLED", True)
+
+INCLUDE_ENABLED = _get_bool("INCLUDE_ENABLED", True)
+
+# allow includes to make an `include()` call.
+INCLUDE_MULTIPLE_LEVEL_ENABLED = False
+
+IMPORT_ENABLED = _get_bool("IMPORT_ENABLED", False)
+
 # Strict mode
 # - Disable the shell (unless really explicit)
 # - Make sure all used files are declared (or just handle this implicitly)
 # - Disable globs/finds
 # - Using paths of another target should be prohibited unless it is an internal (copy/sync/write).
 #   - Any paths of required targets become a dependency and would break composition.
 # - If shell must be enabled, disable __str__ on any PathObject so they can't be hidden in shell strings.
 #   - add concatenate() to explicitly concatenate [shell] strings and any paths they may require.
-STRICT_MODE = False
+STRICT_MODE = _get_bool("STRICT_MODE", False)
 
 if STRICT_MODE:
     SHELL_FUNCTION_ENABLED = False
     GLOB_FUNCTION_ENABLED = False
     FIND_FUNCTION_ENABLED = False
     ENABLE_PATH_TO_STRING = False
```

### Comparing `makex-20240203/python/makex/make_file.py` & `makex-20240401/python/makex/makex_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,341 +1,179 @@
+import ast
 import logging
 import os
 import re
 import shlex
 import shutil
-import sys
-import time
+import types
 from abc import (
     ABC,
     abstractmethod,
 )
-from collections import deque
-from concurrent.futures import (
-    Future,
-    ThreadPoolExecutor,
-)
 from dataclasses import dataclass
 from io import StringIO
 from itertools import chain
 from os import PathLike
 from os.path import (
     expanduser,
     join,
 )
 from pathlib import Path
-from threading import (
-    Event,
-    current_thread,
-)
 from typing import (
     Any,
+    Callable,
     Iterable,
     Optional,
     Pattern,
     Protocol,
     TypedDict,
     Union,
-    Mapping,
 )
 
 from makex._logging import (
     debug,
     error,
     trace,
 )
 from makex.build_path import get_build_path
 from makex.constants import (
-    DIRECT_REFERENCES_TO_MAKEX_FILES,
     ENVIRONMENT_VARIABLES_IN_GLOBALS_ENABLED,
     HASH_USED_ENVIRONMENT_VARIABLES,
+    IGNORE_NONE_VALUES_IN_LISTS,
     OUTPUT_DIRECTLY_TO_CACHE,
     WORKSPACES_IN_PATHS_ENABLED,
 )
 from makex.context import Context
-from makex.errors import ExecutionError
+from makex.errors import (
+    ExecutionError,
+    MakexError,
+)
 from makex.file_checksum import FileChecksum
 from makex.file_system import find_files
 from makex.flags import (
     ABSOLUTE_PATHS_ENABLED,
     ARCHIVE_FUNCTION_ENABLED,
     EXPAND_FUNCTION_ENABLED,
     FIND_FUNCTION_ENABLED,
     FIND_IN_INPUTS_ENABLED,
     GLOB_FUNCTION_ENABLED,
+    GLOBS_IN_ACTIONS_ENABLED,
     GLOBS_IN_INPUTS_ENABLED,
-    GLOBS_IN_RUNNABLES_ENABLED,
     HOME_FUNCTION_ENABLED,
+    IMPORT_ENABLED,
+    INCLUDE_ENABLED,
     NAMED_OUTPUTS_ENABLED,
-    NESTED_WORKSPACES_ENABLED,
     SHELL_USES_RETURN_CODE_OF_LINE,
+    TARGET_PATH_ENABLED,
+)
+from makex.makex_file_types import (
+    AllPathLike,
+    EnvironmentVariableProxy,
+    Expansion,
+    FindFiles,
+    Glob,
+    ListTypes,
+    MultiplePathLike,
+    PathElement,
+    PathLikeTypes,
+    PathObject,
+    RegularExpression,
+    ResolvedTargetReference,
+    TargetReferenceElement,
 )
 from makex.patterns import (
     combine_patterns,
     make_glob_pattern,
 )
 from makex.protocols import (
     CommandOutput,
-    FileProtocol,
     StringHashFunction,
-    TargetProtocol,
 )
 from makex.python_script import (
+    GLOBALS_NAME,
     FileLocation,
     ListValue,
     PythonScriptError,
     PythonScriptFile,
     ScriptEnvironment,
     StringValue,
+    _create_file_location_call,
+    call_function,
+    is_function_call,
     wrap_script_function,
 )
 from makex.run import run
 from makex.target import (
     ArgumentData,
     EvaluatedTarget,
-    TargetKey,
     format_hash_key,
     target_hash,
 )
 from makex.ui import pretty_file
+from makex.version import VERSION
 from makex.workspace import Workspace
+from typing_extensions import (
+    NotRequired,
+    Required,
+    Unpack,
+)
 
-ListTypes = (list, ListValue)
-
-
-class VariableValue:
-    pass
-
-
-class Variable:
-    name: str
-    value: VariableValue
-    location: FileLocation
-
-
-@dataclass(frozen=True)
-class Variant:
-    name: str
-    value: str
-
-
-class RegularExpression:
-    pattern: str
-    location: FileLocation
-
-    def __init__(self, pattern, location):
-        self.pattern = pattern
-        self.location = location
-
-    def __str__(self):
-        return self.pattern
-
-
-class Glob:
-    pattern: StringValue
-    location: FileLocation
-
-    def __init__(self, pattern, location):
-        self.pattern = pattern
-        self.location = location
-
-    def __str__(self):
-        return self.pattern
-
-
-@dataclass()
-class Expansion:
-    """
-    Define a string that will expand according to the shells rules.
-
-    expand("~/.config/path") will exapnd a  user path.
-
-    expand("$VARIABLE") will expand a variable.
-
-    On Unix and Windows, a string that starts with ~ or ~user replaced by that user’s home directory.
-
-    On Unix, an initial ~ is replaced by the environment variable HOME if it is set;
-    otherwise the current user’s home directory is looked up in the password directory through the built-in module pwd.
-    An initial ~user is looked up directly in the password directory.
-
-    On Windows, USERPROFILE will be used if set, otherwise a combination of HOMEPATH and HOMEDRIVE will be used.
-     An initial ~user is handled by checking that the last directory component of the current user’s home directory
-     matches USERNAME, and replacing it if so.
-
-    If the expansion fails or if the path does not begin with a tilde, the path is returned unchanged.
-
-    Substrings of the form $name or ${name} are replaced by the value of environment variable name.
-     Malformed variable names and references to non-existing variables are left unchanged.
-
-    """
-    context: Context
-    string: StringValue
-    location: FileLocation
-
-    # XXX: cache the expanded state
-    _expanded: str = None
-
-    def expand(self, ctx):
-        string = self.string
-        return os.path.expandvars(os.path.expanduser(string))
-
-    def __str__(self):
-        if self._expanded is not None:
-            return self._expanded
-
-        self._expanded = self.expand(self.context)
-        return self._expanded
-
-    def __repr__(self):
-        return f"Expansion({self.string!r})"
-
-
-class PathObject:
-    """
-    The [output] path() object in makex files.
-
-    """
-    def __init__(self, path: Path, location: FileLocation = None):
-        self.path: Path = path
-        self.location = location
-
-    def __str__(self):
-        return self.path.as_posix()
-
-    def __repr__(self):
-        return f"PathObject(path={self.path.as_posix()!r})"
-
-    def __truediv__(self, other):
-        if isinstance(other, StringValue):
-            return PathObject(self.path.joinpath(other.value), other.location)
-        elif isinstance(other, PathObject):
-            return PathObject(self.path / other.path, other.location)
-        else:
-            top = self
-            bottom = other
-            raise TypeError(f"Unsupported operation: {top} / {bottom!r}")
-
-
-class BuildPathVariable:
-    location: FileLocation
-
-    def __init__(self, location=None):
-        self.location = location
-
-    def __str__(self):
-        return "$$$$$$BUILD$$$$$$$"
-
-
-class TargetOutput:
-    def __str__(self):
-        return "$$$$$TARGET-OUTPUT$$$$$"
-
-
-class PathElement:
-    """
-
-    Implements the Path() object as defined in spec.
-
-    Arbitrary paths, relative or absolute.
-
-    """
-    # the original path as defined
-    parts: Union[tuple[str], list[str]] = None
-
-    # Resolved is the actual fully resolved absolute path if any.
-    # XXX: This is an optimization for when we can resolve a path
-    resolved: Path
-
-    location: FileLocation
-
-    # base path of relative paths
-    base: str
-
-    def __init__(self, *args: str, base: str = None, resolved=None, location=None):
-        # TODO: change *args to parts.
-        self.parts = args
-        self.location = location
-        self.resolved = resolved
-        self._path = path = Path(*args)
-        self.base = base
-        if resolved is None:
-            if path.is_absolute():
-                self.resolved = path
-        else:
-            self.resolved = resolved
-
-    @property
-    def name(self):
-        return StringValue(self._path.name, self.location)
-
-    def _as_path(self):
-        return self._path
-
-    if False:
-
-        def absolute(self, _location_: FileLocation = None) -> "PathElement":
-            """
-            Used in the script environment to make paths absolute.
-
-            :param root:
-            :return:
-            """
-
-            # TODO: we should get _line/column/path from the transform call
-            path = Path(*self.parts)
-
-            if not path.is_absolute():
-                path = self.base / path
-
-            return PathElement(*path.parts, resolved=path, location=_location_)
-
-    def __truediv__(self, other):
-        if isinstance(other, StringValue):
-            if self.resolved:
-                _path = Path(other)
-                resolved = self.resolved.joinpath(*_path.parts)
-            else:
-                _path = Path(other)
-                resolved = None
-
-            parts = self.parts + _path.parts
-
-            return PathElement(*parts, resolved=resolved, location=other.location)
-
-        if not isinstance(other, PathElement):
-            raise TypeError(f"Unsupported operation {self} / {other}")
+_TARGET_REFERENCE_NAME = "Reference"
+_MACRO_DECORATOR_NAME = "macro"
 
-        resolved = None
-        if other.resolved and self.resolved:
-            raise TypeError(
-                f"Can't combine two fully absolute resolved Paths. The first path must be absolute, and the other path must be relative \n. Unsupported operation {self} / {other}"
-            )
-        else:
-            if self.resolved:
-                resolved = self.resolved.joinpath(*other.parts)
-            elif other.resolved:
-                raise TypeError("Can't combine unresolved path with resolved path.")
+TARGETS_MODULE_VARIABLE = "_TARGETS_"
+MACROS_MODULE_VARIABLE = "__macros__"
+MACRO_NAMES_MODULE_VARIABLE = "__macro_names__"
+
+DISABLE_ASSIGNMENT_NAMES = {
+    MACROS_MODULE_VARIABLE,
+    MACRO_NAMES_MODULE_VARIABLE,
+    MACRO_NAMES_MODULE_VARIABLE,
+    "target",
+    "Target",
+    _MACRO_DECORATOR_NAME,
+    _TARGET_REFERENCE_NAME,
+    "task",
+    "Task",
+    "path",
+    "execute",
+    "shell",
+    "copy",
+    "print",
+    "E",
+    "ENVIRONMENT",
+    "Environment",
+    "environment",
+    "glob",
+    "pattern",
+    "input",
+    "inputs",
+    "output",
+    "outputs",
+    "find",
+    "Path",
+    "source",
+    "home",
+    "archive",
+    "mirror",
+    "sync",
+    "include",
+}
 
-        parts = self.parts + other.parts
-        return PathElement(*parts, resolved=resolved, location=other.location)
+# TODO: move these to makex_file_types
 
-    def __repr__(self):
-        return f'PathElement({self._as_path()})'
 
-    def __str__(self):
-        if self.resolved:
-            return str(self.resolved)
-        else:
-            raise Exception("Can't use unresolved path here.")
-
-
-def _validate_path(parts: Union[list[str], tuple[str]], location: FileLocation):
+def _validate_path(
+    parts: Union[list[StringValue], tuple[StringValue]],
+    location: FileLocation,
+    absolute=ABSOLUTE_PATHS_ENABLED,
+):
     if ".." in parts:
         raise PythonScriptError("Relative path references not allowed in makex.", location)
-    if ABSOLUTE_PATHS_ENABLED is False and parts[0] == "/":
+    if parts[0] == "/" and absolute is False:
         raise PythonScriptError("Absolute path references not allowed in makex.", location)
     return True
 
 
 VALID_NAME_RE = r"^[a-zA-Z][a-zA-Z0-9\-._@]*"
 VALID_NAME_PATTERN = re.compile(VALID_NAME_RE, re.U)
 
@@ -356,23 +194,23 @@
     base: Path,
 ) -> Path:
     _path = path = Path(element.value)
 
     _validate_path(path.parts, element.location)
 
     if path.parts[0] == "//":
-        trace("Workspace path: %s %s", workspace, element)
+        #trace("Workspace path: %s %s", workspace, element)
         if WORKSPACES_IN_PATHS_ENABLED:
             _path = workspace.path / Path(*path.parts[1:])
         else:
             raise PythonScriptError("Workspaces markers // in paths not enabled.", element.location)
     elif not path.is_absolute():
         _path = base / path
 
-    trace("Resolve string path %s: %s", element, _path)
+    #trace("Resolve string path %s: %s", element, _path)
 
     return _path
 
 
 def resolve_path_element_workspace(
     ctx: Context,
     workspace: Workspace,
@@ -419,35 +257,14 @@
             raise PythonScriptError("Workspaces markers // in paths not enabled.", location)
     elif not path.is_absolute():
         path = base / path
 
     return path
 
 
-class FindFiles:
-    """
-    find files. relative paths are based on the input.
-    """
-    pattern: Union[Glob, RegularExpression]
-    path: Optional[PathElement] = None
-
-    location: FileLocation
-
-    def __init__(self, pattern, path, location):
-        self.pattern = pattern
-        self.path = path
-        self.location = location
-
-
-# TODO: handle bytes
-PathLikeTypes = Union[StringValue, PathElement, PathObject]
-MultiplePathLike = Union[Glob, FindFiles]
-AllPathLike = Union[Glob, FindFiles, StringValue, PathElement]
-
-
 def _string_value_maybe_expand_user(ctx, base, value: StringValue) -> str:
     val = value.value
 
     if False:
         if val.startswith("~"):
             # TODO: use environment HOME to expand the user
             return Path(val).expanduser().as_posix()
@@ -482,14 +299,17 @@
             #pattern = re.compile(pattern)
             ignore = {ctx.output_folder_name}
             #yield from find_files(base, pattern, ignore_names=ignore)
 
             yield from resolve_glob(ctx, target, base, value, ignore_names=ignore)
         elif isinstance(value, PathObject):
             yield value.path
+        elif IGNORE_NONE_VALUES_IN_LISTS and value is None:
+            continue
+
         else:
             #raise ExecutionError(f"{type(value)} {value!r}", target, getattr(value, "location", target))
             raise NotImplementedError(f"Invalid argument in pathlike list: {type(value)} {value!r}")
 
 
 def resolve_string_argument_list(
     ctx: Context,
@@ -498,36 +318,40 @@
     name: str,
     values: Iterable[Union[PathLikeTypes, MultiplePathLike]],
 ) -> Iterable[str]:
     # Used to resolve arguments for an execute command, which must all be strings.
     for value in values:
         if isinstance(value, StringValue):
             # XXX: we're not using our function here because we may not want to expand ~ arguments the way bash does
-            # bash will replace a ~ whereever it is on the command line
+            # bash will replace a ~ wherever it is on the command line
             yield _string_value_maybe_expand_user(ctx, base, value)
         elif isinstance(value, PathObject):
             yield value.path.as_posix()
         elif isinstance(value, PathElement):
             source = resolve_path_element_workspace(ctx, target.workspace, value, base)
             #source = _path_element_to_path(base, value)
             yield source.as_posix()
         elif isinstance(value, Glob):
-            if not GLOBS_IN_RUNNABLES_ENABLED:
-                raise ExecutionError("glob() can't be used in runnables.", target, value.location)
+            if not GLOBS_IN_ACTIONS_ENABLED:
+                raise ExecutionError("glob() can't be used in actions.", target, value.location)
 
             # todo: use glob cache from ctx for multiples of the same glob during a run
             #pattern = make_glob_pattern(value.pattern)
             #pattern = re.compile(pattern)
             ignore = {ctx.output_folder_name}
             #yield from (v.as_posix() for v in find_files(base, pattern, ignore_names=ignore))
             yield from (
                 v.as_posix() for v in resolve_glob(ctx, target, base, value, ignore_names=ignore)
             )
         elif isinstance(value, Expansion):
             yield str(value)
+        elif isinstance(value, tuple):
+            yield from resolve_string_argument_list(ctx, target, base, name, value)
+        elif IGNORE_NONE_VALUES_IN_LISTS and value is None:
+            continue
         else:
             raise NotImplementedError(f"{type(value)} {value!r}")
 
 
 def _resolve_executable_name(ctx: Context, target, base: Path, name, value: StringValue) -> Path:
     if isinstance(value, StringValue):
         return _resolve_executable(ctx, target, value, base)
@@ -558,38 +382,38 @@
         raise NotImplementedError(error_string.format(value=value, target=target))
 
 
 def resolve_glob(
     ctx: Context,
     target: "TargetObject",
     path,
-    pattern: Optional[Union[Glob]],
+    pattern: Glob,
     ignore_names,
 ) -> Iterable[Path]:
     # TODO: check if glob is absolute here?
     glob_pattern = pattern.pattern
-    pattern = re.compile(make_glob_pattern(str(glob_pattern)))
+    _pattern = re.compile(make_glob_pattern(str(glob_pattern)))
 
     yield from find_files(
         path,
-        pattern=pattern,
+        pattern=_pattern,
         ignore_pattern=ctx.ignore_pattern,
         ignore_names=ignore_names,
     )
 
 
 def resolve_find_files(
     ctx: Context,
     target: "TargetObject",
     path,
     pattern: Optional[Union[Glob, StringValue, RegularExpression]],
     ignore_names,
 ) -> Iterable[Path]:
 
-    #TODO: support matchin stringvalues to paths
+    #TODO: support matching stringvalues to paths
     if isinstance(pattern, (Glob, str)):
         pattern = re.compile(make_glob_pattern(str(pattern)))
     elif isinstance(pattern, RegularExpression):
         pattern = re.compile(pattern.pattern, re.U | re.X)
     elif pattern is None:
         pass
     else:
@@ -603,21 +427,38 @@
         pattern=pattern,
         ignore_pattern=ctx.ignore_pattern,
         ignore_names=ignore_names,
     )
 
 
 def _resolve_executable(
-    ctx, target, name: StringValue, base: Path, path_string: str = None
+    ctx,
+    target,
+    name: StringValue,
+    base: Path,
+    path_string: Optional[str] = None,
 ) -> Path:
     if name.find("/") >= 0:
-
+        # path has a slash. resolve using a different algo.
         _path = resolve_string_path_workspace(ctx, target.workspace, name, base)
+        if _path.exists() is False:
+            raise ExecutionError(
+                f"Could not find the executable for {name}. Please install whatever it "
+                f"is that provides the command {name!r}.",
+                target
+            )
         return _path
 
+    path_string = ctx.environment.get("PATH", "")
+    if not path_string:
+        path_string = str(base)
+    else:
+        path_string = f"{base}:{path_string}"
+
+    # XXX: prepend the current folder to the path so executables are found next to the makex file.
     _path = shutil.which(name, path=path_string)
 
     if _path is None:
         error(
             "Which could not find the executable for %r: PATH=%s", name, os.environ.get("PATH", "")
         )
         raise ExecutionError(
@@ -627,16 +468,15 @@
             target
         )
 
     return Path(_path)
 
 
 def create_build_path_object(ctx: Context, target, path, variants, location: FileLocation):
-    workspace = ctx.workspace_path
-
+    # TODO: remove this function. replace with late evaluation.
     path, link_path = get_build_path(
         objective_name=target,
         variants=variants or [],
         input_directory=path,
         build_root=ctx.cache,
         workspace=ctx.workspace_path,
         workspace_id=ctx.workspace_object.id,
@@ -653,79 +493,102 @@
             flatten.extend(v)
         else:
             flatten.append(v)
 
     return target_hash("|".join(flatten))
 
 
-class RunnableElementProtocol(Protocol):
+# TODO: move these to makex_file_actions.py
+
+
+class ActionElementProtocol(Protocol):
     def transform_arguments(self, ctx: Context, target: EvaluatedTarget) -> dict[str, Any]:
         ...
 
     def __call__(self, ctx: Context, target: EvaluatedTarget) -> CommandOutput:
         ...
 
 
-class InternalRunnableBase(ABC):
+class InternalActionBase(ABC):
     location: FileLocation = None
 
+    # TODO: add/collect requirements as we go
+    def add_requirement(self, requirement: "TargetReferenceElement"):
+        raise NotImplementedError
+
+    # TODO: make abstract and wire in.
+    def get_requirements(self, ctx: Context) -> list["TargetReferenceElement"]:
+        """
+        Return a list of any target requirements in the action/arguments. Done before argument transformation.
+
+        Any TargetReference or Path used by the target should be returned (except one for the Target itself).
+
+        Used to detect implicit target requirements.
+        :return:
+        """
+        return []
+
     @abstractmethod
     def transform_arguments(self, ctx: Context, target: EvaluatedTarget) -> ArgumentData:
         # transform the input arguments (stored in instances), to a dictionary of actual values
         # keys must match argument keyword names
         raise NotImplementedError
 
     #implement this with transform_arguments() to get new functionality
     @abstractmethod
     def run_with_arguments(self, ctx: Context, target: EvaluatedTarget, arguments) -> CommandOutput:
         raise NotImplementedError
 
     @abstractmethod
     def hash(self, ctx: Context, arguments: dict[str, Any], hash_function: StringHashFunction):
-        # produce a hash of the runnable with the given arguments and functions
+        # produce a hash of the Action with the given arguments and functions
         # TODO: make abstract once we migrate everything over to the new argument functionality
         raise NotImplementedError
 
     # old stuff below
     def __call__(self, ctx: Context, target: EvaluatedTarget) -> CommandOutput:
         raise NotImplementedError
 
     def __str__(self):
-        return PythonScriptError("Converting Runnable to string not allowed.", self.location)
+        return PythonScriptError("Converting Action to string not allowed.", self.location)
 
 
 @dataclass
-class Execute(InternalRunnableBase):
+class Execute(InternalActionBase):
     executable: PathLikeTypes
     arguments: Union[tuple[AllPathLike], tuple[AllPathLike, ...]]
     environment: dict[str, str]
     location: FileLocation
 
     _redirect_output: PathLikeTypes = None
 
     def transform_arguments(self, ctx: Context, target: EvaluatedTarget) -> ArgumentData:
         args = {}
         args["arguments"] = arguments = []
         target_input = target.input_path
 
         for argument in self.arguments:
             if isinstance(argument, StringValue):
-                arguments.append(_string_value_maybe_expand_user(ctx, target_input, argument))
+                #arguments.append(_string_value_maybe_expand_user(ctx, target_input, argument))
+                arguments.append(argument)
             elif isinstance(argument, PathElement):
                 arguments.append(
                     _resolve_pathlike(ctx, target, target_input, target.name, argument).as_posix()
                 )
             elif isinstance(argument, Expansion):
                 arguments.append(str(argument.expand(ctx)))
             elif isinstance(argument, PathObject):
                 arguments.append(argument.path.as_posix())
             elif isinstance(argument, ListTypes):
                 arguments.extend(
                     resolve_string_argument_list(ctx, target, target_input, target.name, argument)
                 )
+            elif argument is None:
+                # XXX: Ignore None arguments as they may be the result of a condition.
+                continue
             else:
                 raise PythonScriptError(
                     f"Invalid argument type: {type(argument)}: {argument}", target.location
                 )
 
         executable = _resolve_executable_name(
             ctx, target, target_input, target.name, self.executable
@@ -770,15 +633,15 @@
     def hash(self, ctx: Context, arguments: dict[str, Any], hash_function: StringHashFunction):
         _arguments = arguments.get("arguments")
         _executable = arguments.get("executable")
 
         return hash_function("|".join([_executable] + _arguments))
 
 
-class ShellCommand(InternalRunnableBase):
+class Shell(InternalActionBase):
     string: list[StringValue]
     location: FileLocation
 
     # https://pubs.opengroup.org/onlinepubs/9699919799/utilities/V3_chap02.html#tag_18_25
 
     # -e: Error on any error.
     # -u When the shell tries to expand an unset parameter other than the '@' and '*' special parameters,
@@ -795,14 +658,15 @@
 
     def __init__(self, string, location):
         self.string = string
         self.location = location
 
     def transform_arguments(self, ctx: Context, target: EvaluatedTarget) -> ArgumentData:
         args = {}
+        # TODO: validate string type
         args["string"] = self.string
         args["preamble"] = self.preamble
 
         return ArgumentData(args)
 
     def run_with_arguments(self, ctx: Context, target: EvaluatedTarget, arguments) -> CommandOutput:
         string = arguments.get("string")
@@ -830,26 +694,27 @@
             # No subshell is created. The semicolon (or newline) following list is required.
             if SHELL_USES_RETURN_CODE_OF_LINE:
                 _script.append(
                     f"{{ {line}; }} || {{ __error=$?; echo -e \"{ctx.colors.ERROR}Error (exit=$?) on on shell script line {i+1}:{ctx.colors.RESET} {shlex.quote(line)!r}\"; exit $__error; }}"
                 )
             else:
                 _script.append(f"{{ {line}; }}")
-
-            #script.append(f"( {line} ) || (exit $?)")
+                #script.append(f"( {line} ) || (exit $?)")
 
         script = "\n".join(_script)
         trace("Real script:\n%s", script)
-        #stdin = BytesIO()
-        #stdin.write(script.encode("utf-8"))
+
         cwd = target.input_path
         ctx.ui.print(f"Running shell from {cwd}:\n{s_print}\n")
         if ctx.dry_run is True:
             return CommandOutput(0)
         try:
+            #stdin = BytesIO()
+            #stdin.write(script.encode("utf-8"))
+
             # create a real pipe to pass to the specified shell
             read, write = os.pipe()
             os.write(write, script.encode("utf-8"))
             os.close(write)
 
             output = run(
                 [ctx.shell],
@@ -863,55 +728,64 @@
             )
             # XXX: set the location so we see what fails
             # TODO: Set the FileLocation of the specific shell line that fails
             output.location = self.location
             return output
         except Exception as e:
             raise ExecutionError(e, target, location=self.location) from e
-        #finally:
-        #    ctx.ui.print("Script finished")
 
     def hash(self, ctx: Context, arguments: dict[str, Any], hash_function: StringHashFunction):
         return hash_function("\n".join(arguments.get("string", [])))
 
 
 def file_ignore_function(output_folder_name):
     def f(src, names):
         return {output_folder_name}
 
     return f
 
 
 @dataclass
-class Copy(InternalRunnableBase):
+class Copy(InternalActionBase):
     source: Union[list[AllPathLike], PathLikeTypes]
     destination: PathLikeTypes
     exclude: list[AllPathLike]
     location: FileLocation
+    destination_is_subdirectory: bool = False
 
     def hash(self, ctx: Context, arguments: dict[str, Any], hash_function):
         # checksum all the sources
         sources = arguments.get("sources")
 
         # hash the destination name
         destination = arguments.get("destination")
 
         exclusions = arguments.get("exclude", [])
 
         parts = []
         for source in sources:
             parts.append(hash_function(source.as_posix()))
 
-        parts.append(hash_function(destination.as_posix()))
+        if destination is not None:
+            parts.append(hash_function(destination.as_posix()))
 
         if exclusions:
             parts.append(hash_function(exclusions.pattern))
 
         return hash_function("|".join(parts))
 
+    def get_requirements(self, ctx: Context) -> Iterable["TargetReferenceElement"]:
+        if isinstance(self.source, ListTypes):
+            for source in self.source:
+                if isinstance(source, PathObject):
+                    yield source.reference
+        else:
+            if isinstance(self.source, PathObject):
+                yield self.source.reference
+
     def transform_arguments(self, ctx: Context, target: EvaluatedTarget) -> ArgumentData:
         if isinstance(self.source, ListTypes):
             sources = list(
                 resolve_pathlike_list(
                     ctx=ctx,
                     target=target,
                     name="source",
@@ -927,23 +801,32 @@
                     name="source",
                     base=target.input_path,
                     value=self.source
                 )
             ]
 
         if self.destination:
+
+            if not isinstance(self.destination, (str, PathObject, PathElement)):
+                raise PythonScriptError("Destination must be a string or path.", self.location)
+
+            if isinstance(self.destination, str):
+                if "/" in self.destination:
+                    self.destination_is_subdirectory = True
+
             destination = _resolve_pathlike(
                 ctx=ctx,
                 target=target,
                 name="destination",
                 base=target.path,
                 value=self.destination
             )
+
         else:
-            destination = target.path
+            destination = None
 
         excludes = None
         if self.exclude:
             excludes = []
             pattern_strings = []
             if isinstance(self.exclude, ListValue):
                 pattern_strings = self.exclude
@@ -970,17 +853,24 @@
     def run_with_arguments(
         self, ctx: Context, target: EvaluatedTarget, arguments: ArgumentData
     ) -> CommandOutput:
         sources = arguments.get("sources")
         destination: Path = arguments.get("destination")
         excludes: Pattern = arguments.get("excludes")
 
+        destination_specified = destination is not None
+        if destination_specified:
+            destination_is_folder = destination.is_dir()
+        else:
+            destination = target.path
+            destination_is_folder = True
+
         copy_file = ctx.copy_file_function
 
-        if not destination.exists():
+        if destination.exists() is False:
             debug("Create destination %s", destination)
             if ctx.dry_run is False:
                 destination.mkdir(parents=True)
 
         length = len(sources)
         if length == 1:
             ctx.ui.print(f"Copying to {destination} ({sources[0]})")
@@ -1002,31 +892,63 @@
                     trace("Copy/ignore: %s", path)
                     _names.add(name)
                 elif excludes and excludes.match(path):
                     trace("Copy/exclude: %s", path)
                     _names.add(name)
             return _names
 
-        # sometimes
+        # XXX: keep n sources so we can determine which form of copy() we have (8 forms).
+        #  copy(items) will always use the file/folder name in the items list
+        #  copy(files)
+        #  copy(file)
+        #  copy(folders)
+        #  copy(folder)
+        # with destination:
+        #  copy(file, file) copy a file to specified file path. TODO: this doesn't work. remove this. suggest install()
+        #  copy(file, folder) copy a file to specified folder.
+        #  copy(folder, folder) allows renaming or mirroring a folder.
+        #  copy(folders, folder) copies a set of folders to the specified folder..
+        #  copy(files, folder) copies a set of files to the specified folder.
+
+        #  copy(file, "folder" / file) allows renaming a file and prefixing it into a folder. TODO: remove this. suggest install()
+        n_sources = len(sources)
+
         for source in sources:
 
             if not source.exists():
                 raise ExecutionError(
                     f"Missing source file {source} in copy list",
                     target,
                     getattr(source, "location", target.location)
                 )
 
             if ignore_pattern.match(source.as_posix()):
                 trace("File copy ignored %s", source)
                 continue
 
             #trace("Copy source %s", source)
-            if source.is_dir():
+            if destination_specified:
+                # destination was specified, one of:
+                # copy(folder, folder)
+                # copy(folders, folder)
+                # copy(file, file)
+                # copy(files, destination)
+                if n_sources == 1:
+                    _destination = destination
+                else:
+                    _destination = destination / source.name
+            else:
+                # destination not specified, one of:
+                # copy(folder)
+                # copy(folders)
+                # copy(file)
+                # copy(files)
                 _destination = destination / source.name
+
+            if source.is_dir():
                 debug("Copy tree %s <- %s", _destination, source)
 
                 if ctx.dry_run is False:
                     try:
                         # copy recursive
                         shutil.copytree(
                             source,
@@ -1044,40 +966,37 @@
                             for error in tup:
                                 e_source, e_destination, exc = error
                                 string.append(
                                     f"\tError copying to  {e_destination} from {e_source}\n\t\t{exc} {copy_file}"
                                 )
                         if ctx.debug:
                             logging.exception(e)
-                        string = "\n".join(string)
-                        raise ExecutionError(string, target, target.location) from e
+                        raise ExecutionError("\n".join(string), target, target.location) from e
                     except OSError as e:
                         string = [
                             f"Error copying tree {source} to {destination}:\n  Error to {e.filename} from {e.filename2}: {type(e)}: {e.args[0]} {e} "
                         ]
 
-                        string = "\n".join(string)
-                        raise ExecutionError(string, target, target.location) from e
+                        raise ExecutionError("\n".join(string), target, target.location) from e
             else:
-                trace("Copy file %s <- %s", destination / source.name, source)
+                trace("Copy file %s <- %s", _destination, source)
                 if ctx.dry_run is False:
                     try:
-                        copy_file(source.as_posix(), (destination / source.name).as_posix())
-
+                        copy_file(source.as_posix(), _destination.as_posix())
                     except (OSError, shutil.Error) as e:
                         raise ExecutionError(
-                            f"Error copying file {source} to {destination/source.name}: {e}",
+                            f"Error copying file {source} to {_destination}: {e}",
                             target,
                             target.location
                         ) from e
         return CommandOutput(0)
 
 
 @dataclass
-class Synchronize(InternalRunnableBase):
+class Synchronize(InternalActionBase):
     """
         synchronize/mirror files much like rsync.
 
         list of input paths are mirrored to Target.path
         e.g.
         sync(["directory1", "file1", "sub/directory"])
 
@@ -1110,123 +1029,105 @@
             raise PythonScriptError(
                 f"Source argument is empty.",
                 self.location,
             )
 
         _source_list = self.source
 
-        try:
-            _source_list = iter(_source_list)
-        except TypeError:
-            # make it iterable and try.
-            _source_list = [_source_list]
-            if False:
-                # not iterable
-                raise PythonScriptError(
-                    f"Expected variable number of sources, got {type(_source_list)}: {_source_list!r}",
-                    getattr(_source_list, "location", self.location)
-                )
+        if isinstance(self.source, (list, ListValue)):
+            _source_list = self.source
         else:
-            # iterable
-            pass
-
-        #if not isinstance(self.source, ListTypes):
-        #    raise PythonScriptError(
-        #        f"Expected variable number of sources, got {type(self.source)}: {self.source!r}", getattr(self.source, "location", self.location)
-        #    )
+            _source_list = [self.source]
 
         args["sources"] = sources = list(
             resolve_pathlike_list(
                 ctx=ctx,
                 target=target,
                 name="source",
                 base=target.input_path,
                 values=_source_list,
-                glob=GLOBS_IN_RUNNABLES_ENABLED,
+                glob=GLOBS_IN_ACTIONS_ENABLED,
             )
         )
-        trace("Synchronize sources %s", sources)
+        #trace("Synchronize sources %s", sources)
 
         if self.destination:
             destination = _resolve_pathlike(
                 ctx=ctx,
                 target=target,
                 name="destination",
                 base=target.path,
                 value=self.destination
             )
-            if ctx.dry_run is False:
-                destination.mkdir(parents=True, exist_ok=True)
         else:
             destination = target.path
-            if ctx.dry_run is False:
-                destination.mkdir(parents=True, exist_ok=True)
 
         args["destination"] = destination
         args["symlinks"] = self.symlinks
 
         return ArgumentData(args)
 
     def run_with_arguments(self, ctx: Context, target: EvaluatedTarget, arguments) -> CommandOutput:
         sources: list[Path] = arguments.get("sources")
         destination: Path = arguments.get("destination")
         symlinks: Path = arguments.get("symlinks")
 
         ignore = file_ignore_function(ctx.output_folder_name)
 
+        if ctx.dry_run is False:
+            destination.mkdir(parents=True, exist_ok=True)
+
         debug("Synchronize to destination: %s", destination)
 
         length = len(sources)
 
         if length > 1:
-            ctx.ui.print(f"Synchonizing to {destination} ({length} items)")
+            ctx.ui.print(f"Synchronizing to {destination} ({length} items)")
         else:
-            ctx.ui.print(f"Synchonizing to {destination} ({sources[0]})")
+            ctx.ui.print(f"Synchronizing to {destination} ({sources[0]})")
 
         for source in sources:
             #trace("Synchronize source to destination: %s: %s", source, destination)
             if not source.exists():
                 raise ExecutionError(
                     f"Missing source/input file {source} in sync()", target, location=self.location
                 )
-            if source.is_dir():
-                # Fix up destination; source relative should match destination relative.
-                if source.is_relative_to(target.input_path):
-                    _destination = destination / source.relative_to(target.input_path)
-                    if ctx.dry_run is False:
-                        _destination.mkdir(parents=True, exist_ok=True)
-                else:
-                    _destination = destination
 
-                trace("Copy tree %s <- %s", _destination, source)
+            # Fix up destination; source relative should match destination relative.
+            if source.parent.is_relative_to(target.input_path):
+                _destination = destination / source.parent.relative_to(target.input_path)
+
                 if ctx.dry_run is False:
-                    # copy recursive
-                    shutil.copytree(source, _destination, dirs_exist_ok=True, ignore=ignore)
+                    _destination.mkdir(parents=True, exist_ok=True)
             else:
-                if source.parent.is_relative_to(target.input_path):
-                    _destination = destination / source.parent.relative_to(target.input_path)
-
-                    if ctx.dry_run is False:
-                        _destination.mkdir(parents=True, exist_ok=True)
+                _destination = destination
 
+            if source.is_dir():
+                # copy recursive
+                trace("Copy tree %s <- %s", _destination, source)
+                if ctx.dry_run:
+                    continue
+                shutil.copytree(source, _destination, dirs_exist_ok=True, ignore=ignore)
+            else:
                 trace("Copy file %s <- %s", _destination / source.name, source)
-                if ctx.dry_run is False:
-                    shutil.copy(source, _destination / source.name)
+                if ctx.dry_run:
+                    continue
+                shutil.copy(source, _destination / source.name)
 
         return CommandOutput(0)
 
     def hash(self, ctx: Context, arguments: dict[str, Any], hash_function: StringHashFunction):
         parts = [self.__class__.__name__, arguments.get("destination").as_posix()]
         parts.extend([a.as_posix() for a in arguments.get("sources")])
 
         return hash_function("|".join(parts))
 
 
 @dataclass
-class Print(InternalRunnableBase):
+class Print(InternalActionBase):
     messages: list[str]
 
     def __init__(self, messages, location):
         self.messages = messages
         self.location = location
 
     def run_with_arguments(self, ctx: Context, target: EvaluatedTarget, arguments) -> CommandOutput:
@@ -1240,22 +1141,26 @@
 
     def hash(self, ctx: Context, arguments: dict[str, Any], hash_function: StringHashFunction):
         # this hash doesn't matter; doesn't affect output
         return ""
 
 
 @dataclass
-class Write(InternalRunnableBase):
+class Write(InternalActionBase):
     path: PathLikeTypes
     data: StringValue
+    executable: bool = False
 
-    def __init__(self, path: PathLikeTypes, data: StringValue = None, location=None):
+    def __init__(
+        self, path: PathLikeTypes, data: StringValue = None, executable=False, location=None
+    ):
         self.path = path
         self.data = data
         self.location = location
+        self.executable = False
 
     def transform_arguments(self, ctx: Context, target: EvaluatedTarget) -> ArgumentData:
         args = {}
         args["path"] = path = _resolve_pathlike(ctx, target, target.path, "path", self.path)
 
         data = self.data
         if isinstance(data, StringValue):
@@ -1266,46 +1171,54 @@
             raise ExecutionError(
                 f"Invalid argument text argument to write(). Got {data!r} {type(data)}. Expected string.",
                 target,
                 location=getattr(data, "location", target.location)
             )
 
         args["data"] = data
+        args["executable"] = self.executable
         return ArgumentData(args, inputs=[path])
 
     def run_with_arguments(self, ctx: Context, target: EvaluatedTarget, arguments) -> CommandOutput:
-        path = arguments.get("path")
+        path: Path = arguments.get("path")
         data = arguments.get("data")
 
         ctx.ui.print(f"Writing {path}")
 
+        if ctx.dry_run is False:
+            if not path.parent.exists():
+                path.parent.mkdir(mode=0o755, parents=True)
+
         if data is None:
             debug("Touching file at %s", path)
             if ctx.dry_run is False:
                 path.touch(exist_ok=True)
         elif isinstance(data, str):
             debug("Writing file at %s", path)
             if ctx.dry_run is False:
                 path.write_text(data)
         else:
             raise ExecutionError(
-                "Invalid argument text argument to write()", target, location=target.location
+                "Invalid argument data argument to write()", target, location=target.location
             )
 
+        if self.executable:
+            path.chmod(0o755)
+
         return CommandOutput(0)
 
     def hash(self, ctx: Context, arguments: dict[str, Any], hash_function: StringHashFunction):
         parts = [
             arguments.get("path").as_posix(),
             arguments.get("data"),
         ]
         return hash_function("|".join(parts))
 
 
-class SetEnvironment(InternalRunnableBase):
+class SetEnvironment(InternalActionBase):
     environment: dict[StringValue, Union[StringValue, PathLikeTypes]]
 
     def __init__(self, environment: dict, location: FileLocation):
         self.environment = environment
         self.location = location
 
     def transform_arguments(self, ctx: Context, target: EvaluatedTarget) -> ArgumentData:
@@ -1338,111 +1251,198 @@
 
     def hash(self, ctx: Context, arguments: dict[str, Any], hash_function: StringHashFunction):
         environment = arguments.get("environment")
         environment_string = ";".join(f"{k}={v}" for k, v in environment.items())
         return hash_function(environment_string)
 
 
-@dataclass
-class TargetReferenceElement:
+class InsertAST(ast.NodeTransformer):
+    def __init__(self, path, asts: list[ast.AST]):
+        self.path = path
+        self.asts = asts
+
+    def visit_Module(self, node: ast.Module) -> Any:
+        node.body = self.asts + node.body
+
+
+class ProcessIncludes(ast.NodeTransformer):
     """
-    A reference to a target in a makex file: Target(name, path).
+        Adds a globals() argument to include() calls so that the environment can modify its own globals.
 
-    Also produced synthetically when : is called.
+
+        TODO: includes should be at the top of the file; enforcing this is tricky.
+        we need to scan the body for any include() calls.
+        if any include() is found after any other statement, raise an error
     """
-    name: StringValue
-    path: Union[PathElement, StringValue] = None
-    location: FileLocation = None
+    def __init__(self, path: str):
+        self.path = path
+        self.includes_seen: list[tuple[str, FileLocation]] = []
 
-    def __repr__(self):
-        path = self.path
-        if path is not None:
-            return f"TargetReferenceElement({self.name.value!r}, {path!r})"
+    def visit_Call(self, node: ast.Call) -> Any:
+        if is_function_call(node, "include") is False:
+            return node
+
+        line = node.lineno
+        col = node.col_offset
+
+        #location = FileLocation(line, col, self.path)
+        #if other_nodes_seen:
+        #    raise PythonScriptError("Includes must be at the top of a file.", location)
+        #else:
+        #self.includes_seen.append((node.args[0].value, location))
 
-        return f"TargetReferenceElement({self.name.value!r})"
+        node.keywords.append(
+            ast.keyword(
+                arg='_globals',
+                value=call_function(GLOBALS_NAME, line, col),
+                lineno=line,
+                col_offset=col,
+            )
+        )
+        #debug("Transform include %s", ast.dump(node))
+        return node
 
 
-@dataclass
-class ResolvedTargetReference:
-    """
-    Used in a target graph and for external matching.
+class TransformGetItem(ast.NodeTransformer):
     """
-    name: StringValue
+        Transforms Target Reference Slice Syntax: Target[path:name] into a TargetReference(name, path)
 
-    # path the actual makex file containing the target
-    path: Path
 
-    # where this reference was defined
-    location: FileLocation = None
+    >>> print(ast.dump(ast.parse('target["test":"test":"test"]', mode='single'), indent=4))
 
-    def key(self):
-        return format_hash_key(self.name, self.path)
-
-    def __eq__(self, other):
-        #assert isinstance(other, ResolvedTargetReference), f"Got {type(other)} {other}. Expected ResolvedTarget"
-        assert hasattr(other, "key"), f"{other!r} has no key() method."
-        assert callable(getattr(other, "key"))
-        return self.key() == other.key()
+        Subscript(
+            value=Name(id='target', ctx=Load()),
+            slice=Slice(
+                lower=Constant(value='test'),
+                upper=Constant(value='test'),
+                step=Constant(value='test')),
+            ctx=Load()
+            )
+        )
+    """
+    NAME = "Target"
 
-    def __hash__(self):
-        return hash(self.key())
+    def __init__(self, path):
+        super().__init__()
+        self.path = str(path)
+
+    def visit_Subscript(self, node: ast.Subscript) -> Any:
+        if isinstance(node.value, ast.Name) is False:
+            self.generic_visit(node)
+            return node
+        if node.value.id != self.NAME:
+            self.generic_visit(node)
+            return node
+
+        line = node.lineno
+        offset = node.col_offset
+        slice: ast.Slice = node.slice
+
+        lower = slice.lower or ast.Constant(None, lineno=line, col_offset=offset)
+        upper = slice.upper or ast.Constant(None, lineno=line, col_offset=offset)
+        step = slice.step or ast.Constant(None, lineno=line, col_offset=offset)
+
+        file_location = _create_file_location_call(self.path, line, offset)
+
+        reference_call = ast.Call(
+            func=ast.Name(
+                id=_TARGET_REFERENCE_NAME,
+                ctx=ast.Load(),
+                lineno=line,
+                col_offset=offset,
+            ),
+            args=[],
+            keywords=[
+                ast.keyword(
+                    arg='name',
+                    value=upper,
+                    lineno=line,
+                    col_offset=offset,
+                ),
+                ast.keyword(
+                    arg='path',
+                    value=lower,
+                    lineno=line,
+                    col_offset=offset,
+                ),
+                ast.keyword(
+                    arg='location',
+                    value=file_location,
+                    lineno=line,
+                    col_offset=offset,
+                ),
+            ],
+            lineno=line,
+            col_offset=offset,
+        )
+        return reference_call
 
 
 class TargetObject:
     name: StringValue
     path: PathElement
     requires: list[Union[PathElement, PathObject, "TargetObject"]]
-    commands: list[RunnableElementProtocol]
+    commands: list[ActionElementProtocol]
+
+    # TODO: inputs dictionary, "" or None is for unnamed inputs
+    inputs: dict[None, AllPathLike]
 
     # outputs as a list. fast checks if has any outputs
     outputs: list[PathElement]
 
     # named outputs dict
     # None key is unnamed outputs
     outputs_dict: dict[Union[None, str], list[Union[PathElement, PathObject]]]
 
-    # location to build. can be overidden by users.
+    # location to build. can be overridden by users.
     build_path: Path
 
+    # The location in which this task was actually defined (i.e. where the task() function was called).
     location: FileLocation
 
     resolved_requires: list[ResolvedTargetReference]
 
     workspace: Workspace
 
     #makex_file_checksum: str
 
+    # The makex file in which this target was registered
     makex_file: "MakexFile"
 
+    endless: bool = False
+
     def __init__(
         self,
         name,
         path: Union[StringValue, PathElement] = None,
         requires=None,
         run=None,
         outputs=None,
         build_path=None,
         outputs_dict=None,
         workspace=None,
         #makex_file_checksum=None,
         makex_file=None,
+        # TODO: pass the includer file so we can distinguish between where a target was defined and where it was finally included
+        #   we need to use the includer to generate target.keys()
+        includer=None,
         location=None,
     ):
         #if not path is None:
         #    assert isinstance(path, (PathElement)), f"Got: {path!r}"
 
         self.name = name
         self.path = path
         self.requires = requires or []
         self.commands = run or []
         self.outputs = outputs or []
         self.build_path = build_path
         self.workspace = workspace
 
-        # cache the requirement references weve obtained so we don't have to search for makex file later
+        # cache the requirement references we've obtained so we don't have to search for makex file later
         self.resolved_requires = []
         self.outputs_dict = outputs_dict or {}
 
         if outputs and outputs_dict is None:
             # TEST ONLY
             for output in outputs:
                 self.outputs_dict.setdefault(None, []).append(output)
@@ -1450,60 +1450,56 @@
         self.makex_file = makex_file
 
         self.location = location
 
     def all_outputs(self) -> Iterable[Union[PathElement, PathObject]]:
         d = self.outputs_dict
         if not d:
-            return
+            return None
+
         yield from d.get(None)
 
         for k, v in d.items():
-            yield from v
+            if isinstance(v, list):
+                yield from v
+            else:
+                yield v
 
     def add_resolved_requirement(self, requirement: ResolvedTargetReference):
         self.resolved_requires.append(requirement)
 
     @property
     def makex_file_path(self) -> str:
-        return self.location.path
+        return self.makex_file.path.as_posix()
 
     def path_input(self):
-        return Path(self.location.path).parent
+        """ Return the directory where this target is declared/applicable. """
+        return self.makex_file.directory
 
     def __eq__(self, other):
         if not isinstance(other, (TargetObject, ResolvedTargetReference)):
             return False
 
         return self.key() == other.key()
-        #return other.path == self.path and self.name == other.name
 
     def key(self):
-        #if self.path is None or self.path.resolved:
-        #    raise Exception(f"Can't hash key of unresovled {self!r}")
-
-        return format_hash_key(self.name, self.location.path)
-
-        #return hash_target(self)
+        return format_hash_key(self.name, self.makex_file.path)
 
     def __hash__(self):
-
-        #if self.path is None:
-        #    return hash(f":{self.name}:")
-
-        #if not self.path.as_path():
-        #    raise Exception(f"Can't hash unresolved path {self.path}")
-
         return hash(self.key())
 
     def __repr__(self):
         if self.path:
-            return f"TargetObject(\"{self.name}\", {self.location.path})"
+            return f"TargetObject(\"{self.name}\", {self.makex_file.path})"
         return f"TargetObject(\"{self.name}\")"
 
+    def for_include(self, file: "MakexFile"):
+        # return a target transformed for inclusion
+        raise NotImplementedError
+
 
 def resolve_target_output_path(ctx, target: TargetObject):
     # return link (or direct) and cache path.
     target_input_path = target.path_input()
 
     if target.path is None:
         build_path, linkpath = get_build_path(
@@ -1554,15 +1550,15 @@
         )
     else:
         raise NotImplementedError(f"{type(target)} {target!r}")
 
     return target_output_path, real_path
 
 
-class MakexFileCycleError(Exception):
+class MakexFileCycleError(MakexError):
     detection: TargetObject
     cycles: list[TargetObject]
 
     def __init__(self, message, detection: TargetObject, cycles: list[TargetObject]):
         super().__init__(message)
         self.message = message
         self.detection = detection
@@ -1589,390 +1585,171 @@
             string.write("Stack:\n")
             for r in stack:
                 string.write(f" - {r}\n")
 
         return string.getvalue()
 
 
-class TargetGraph:
-    # NOTE: We use TargetObject here because we use isinstance checks
-
-    targets: list[TargetObject]
-
-    def __init__(self):
-        # TODO: we could probably merge TargetKey and file keys and all of these dictionaries.
-
-        # TargetKey -> object
-        self.targets: dict[TargetKey, TargetObject] = {}
-
-        # map of TargetKey to all of it's requirements
-        self._requires: dict[TargetKey, list[TargetObject]] = {}
-
-        # map of TargetKey to all the Files/paths it provides
-        self._provides: dict[TargetKey, list[PathLike]] = {}
-
-        # map from all the files inputting into TargetObject
-        self._files_to_target: dict[PathLike, set[TargetObject]] = {}
-
-        # map from TargetKey to all the things it provides to
-        self._provides_to: dict[TargetKey, set[TargetObject]] = {}
-
-    def __contains__(self, item: ResolvedTargetReference):
-        return item.key() in self.targets
-
-    def get_target(self, t) -> Optional[TargetObject]:
-        #debug("Find %s in %s. key=%s", t, self.targets, t.key())
-        return self.targets.get(t.key(), None)
-
-    def in_degree(self) -> Iterable[tuple[TargetObject, int]]:
-        for key, target in self.targets.items():
-            yield (target, len(self._provides_to.get(key, [])))
-
-    def add_targets(self, ctx: Context, *targets: TargetObject):
-        assert isinstance(ctx, Context)
-        assert ctx.workspace_object
-
-        for target in targets:
-            self.add_target(ctx, target)
-
-    def _process_target_requirements(
-        self,
-        ctx: Context,
-        target: TargetObject,
-    ) -> Iterable[TargetObject]:
-
-        target_input_path = target.path_input()
-        makex_file_path = Path(target.location.path)
-
-        for require in target.requires:
-            if isinstance(require, PathElement):
-                # a simple path to a file.. declared as Path() or automatically parsed
-                # resolve the input file path
-                if False:
-                    path = require._as_path()
-
-                    if not path.is_absolute():
-                        # make path relative to target
-                        path = target_input_path / path
-
-                path = resolve_path_element_workspace(
-                    ctx, target.workspace, require, target_input_path
-                )
-
-                # point file -> current target
-                self._files_to_target.setdefault(path, set()).add(target)
-                continue
-            elif isinstance(require, TargetObject):
-                # add to rdeps map
-                self._provides_to.setdefault(require.key(), set()).add(target)
-                # add to requires map
-                #requirements.append(require)
-                # TODO: this is for tests only. should yield a ResolvedTargetReference
-                yield require
-            elif isinstance(require, TargetReferenceElement):
-                # reference to a target, either internal or outside the makex file
-                name = require.name.value
-                path = require.path
-
-                #trace("reference input is %r: %r", require, path)
-
-                location = require.location
-                if isinstance(path, StringValue):
-                    # Target(name, "some/path")
-                    location = path.location
-                    #_path = Path(path.value)
-                    _path = resolve_string_path_workspace(
-                        ctx, target.workspace, path, target_input_path
-                    )
-                elif isinstance(path, PathElement):
-                    # Target(name, Path())
-                    location = path.location
-
-                    _path = resolve_path_element_workspace(
-                        ctx, target.workspace, path, target_input_path
-                    )
-                elif path is None:
-                    # Target(name)
-                    _path = makex_file_path
-                elif isinstance(path, str):
-                    # XXX: this is used for testing only. we should not be dealing with str (instead we should a StringValues)
-                    location = FileLocation(None, None, target.location)
-                    _path = Path(path)
-                else:
-                    raise ExecutionError(
-                        f"Invalid target reference path: Type: {type(path)} {path}",
-                        target,
-                        getattr(path, "location", None)
-                    )
-
-                if not _path.is_absolute():
-                    _path = target_input_path / _path
-
-                if _path.is_dir():
-                    # find the makexfile it's referring to
-                    file = find_makex_files(_path, ctx.makex_file_names)
-                    if file is None:
-                        raise ExecutionError(
-                            f"No makex file found at {_path}. Invalid target reference.",
-                            target,
-                            path.location
-                        )
-                else:
-                    file = _path
-
-                #trace("Got reference %r %r", name, file)
-                #requirements.append(ResolvedTargetReference(name, path))
-                yield ResolvedTargetReference(name, file, location=location)
-            elif isinstance(require, (FindFiles, Glob)):
-                # These things will be resolved in a later pass.
-                # TODO: we may want to resolve these early and keep a cache.
-                pass
-            else:
-                raise NotImplementedError(f"Type: {type(require)}")
-
-    def add_target(self, ctx: Context, target: TargetObject):
-        # add targetobjects during parsing
-
-        # add all the targets we encountered during evaluation
-        self.targets[target.key()] = target
-
-        key = target.key()
-        self._requires[key] = requirements = []
-
-        if target.requires:
-            #### process the requirements, a list of PathElement(input file) | StringValue | Target
-            for requirement in self._process_target_requirements(ctx, target):
-                requirements.append(requirement)
-
-        self._provides[key] = provides = []
-
-        #trace("Add target to graph: %r", target)
-        output_path, real_path = resolve_target_output_path(ctx, target)
-
-        if output_path:
-            pass
-
-        if target.outputs:
-            for output in target.all_outputs():
-                if isinstance(output, PathElement):
-                    output = resolve_path_element_workspace(
-                        ctx, target.workspace, output, output_path
-                    )
-                    #output = output._as_path()
-
-                    #if not output.is_absolute():
-                    # make path relative to target
-                    #    output = output_path / output
-                elif isinstance(output, PathObject):
-                    output = output.path
-                elif isinstance(output, StringValue):
-                    output = Path(output.value)
-
-                    if not output.is_absolute():
-                        # make path relative to target
-                        output = output_path / output
-
-                elif isinstance(output, (FindFiles, Glob)):
-                    pass
-                else:
-                    raise NotImplementedError(f"Invalid output type {type(output)} {output}")
-
-                provides.append(output)
-
-    def get_requires(
-        self,
-        target: TargetProtocol,
-        recursive=False,
-        _seen: set = None,
-    ) -> Iterable[TargetObject]:
-        # XXX: faster version of get_requires without cycle detection. used by the executor/downstream
-        # query the graph for requirements in reverse order (farthest to closest)
-        # TODO: we should be able to remove _seen entirely.
-        _seen = set() if _seen is None else _seen
-
-        if target in _seen:
-            return
-
-        _seen.add(target)
-
-        for requirement in self._requires.get(target.key(), []):
-            if requirement in _seen:
-                continue
-
-            if recursive:
-                yield from self.get_requires(requirement, recursive=recursive, _seen=_seen)
-
-            yield requirement
-
-    def get_requires_detect_cycles(
-        self,
-        target: TargetProtocol,
-        recursive=False,
-        _stack: list = None,
-        _seen: set = None
-    ) -> Iterable[TargetObject]:
-        # query the graph for requirements in reverse order (farthest to closest)
-        _stack = list() if _stack is None else _stack
-        _seen = set() if _seen is None else _seen
-
-        #trace("Get requires and detect cycles %r", target)
-        if target in _stack:
-            return
-
-        _stack.append(target)
-
-        _seen.add(target)
-
-        for requirement in self._requires.get(target.key(), []):
-            requirement: TargetObject = requirement
-
-            if requirement in _seen:
-                continue
-
-            if requirement in _stack:
-                #error("CYCLES %r: %r", requirement, _seen)
-                target = self.targets.get(requirement.key())
-                # reverse so we see the most recent file depended on.
-                reverse = [self.targets.get(s.key()) for s in reversed(_stack)]
-                raise MakexFileCycleError(
-                    f"Internal cycle detected: {requirement!r}", target, reverse
-                )
-
-            if recursive:
-                yield from self.get_requires_detect_cycles(
-                    requirement, recursive=recursive, _stack=_stack, _seen=_seen
-                )
-
-            yield requirement
-
-        _stack.pop()
-
-    def get_outputs(self, *targets, recursive=False) -> Iterable[FileProtocol]:
-        # reverse dependencies of targets
-        # targets outputs + outputs for each of targets.requires
-        for target in targets:
-            yield from self._provides.get(target, [])
-
-            if recursive:
-                yield from self.get_outputs(target.requires)
-
-    def topological_sort_grouped(self: "TargetGraph", start: list[TargetObject]):
-        indegree_map = {v: d for v, d in self.in_degree() if d > 0}
-        zero_indegree = [v for v, d in self.in_degree() if d == 0]
-
-        while zero_indegree:
-            yield zero_indegree
-            new_zero_indegree = []
-            for v in zero_indegree:
-                for child in self.get_requires_detect_cycles(v):
-                    indegree_map[child] -= 1
-                    if not indegree_map[child]:
-                        new_zero_indegree.append(child)
-            zero_indegree = new_zero_indegree
-
-
-def find_makex_files(path, names):
+def find_makex_files(path, names) -> Optional[Path]:
     for name in names:
         check = path / name
         if check.exists():
             return check
     return None
 
 
 @dataclass
 class ArchiveCommand:
     path: PathLike
     prefix: PathLike
     location: FileLocation
 
 
-class FileObject(FileProtocol):
-    path: PathLike
-    location: FileLocation
-
-
-SENTINEL = object()
-
+class IncludeFunction(Protocol):
+    def __call__(
+        self,
+        ctx: Context,
+        workspace: Workspace,
+        base: Path,
+        search_path: str,
+        makex_file: "MakexFile",
+        location: FileLocation,
+        search=False,
+        globals=None,
+        stack=None,
+        targets=False,
+        required=True,
+    ) -> tuple[types.ModuleType, "MakexFile"]:
+        pass
 
-class EnvironmentProxy:
-    def __init__(self, env):
-        self.__env = env
-        # record usages of environment variables so we can include it as part of the hashing of targets/makex files.
-        self.__usages: dict[str, str] = {}
 
-    def get(self, key, default=SENTINEL, _location_: FileLocation = None):
-        item = self.__env.get(key, default)
-        if item is None or item is SENTINEL:
-            raise PythonScriptError(f"Enviroment variable {key} not defined.", _location_)
+def _process_output(
+    output: Union[StringValue, Glob],
+    target_name,
+    location,
+) -> Union[PathElement, PathObject, Glob]:
+    # Mostly return the outputs, as is, for later evaluation. Check for invalid arguments early.
+    if isinstance(output, StringValue):
+        return PathElement(output, location=output.location)
+    elif isinstance(output, Glob):
+        # append glob as is. we'll resolve later.
+        return output
+    elif isinstance(output, PathObject):
+        return output
+    elif isinstance(output, PathElement):
+        return output
+    else:
+        raise PythonScriptError(
+            f"Invalid output type {type(output)} in output list for target {target_name}: {output}",
+            location
+        )
 
-        self.__usages[key] = item
 
-        return StringValue(item, location=_location_)
+class MakexFileScriptEnvironment(ScriptEnvironment):
+    class Task:
+        def __init__(self, env):
+            self.env = env
+
+        def __getitem__(self, item):
+            if item not in {"path"}:
+                raise AttributeError
 
-    def _usages(self):
-        return self.__usages
+            return self.env.path
 
+        def __call__(self, *args, **kwargs):
+            pass
 
-class MakefileScriptEnv(ScriptEnvironment):
     def __init__(
         self,
         ctx,
         directory: Path,
         path: Path,
         workspace: Workspace = None,
-        checksum: str = None,
-        targets: dict[str, TargetObject] = None,
-        makex_file: "MakexFile" = None,
+        targets: Optional[dict[str, TargetObject]] = None,
+        macros: Optional[dict[str, Callable]] = None,
+        makex_file: Optional["MakexFile"] = None,
+        stack: Optional[list[str]] = None, # stack of paths reaching the file
+        include_function: Optional[IncludeFunction] = None,
+        globals=None,
     ):
+        self.stack = stack or [path.as_posix()]
+
         self.directory = directory
 
         # path to the actual makex file
         self.path = path
 
         self.ctx = ctx
         # TODO: wrap environment dict so it can't be modified
-        self.environment = EnvironmentProxy(ctx.environment)
+        self.environment = EnvironmentVariableProxy(ctx.environment)
         self.targets = {} if targets is None else targets
         #self.variables = []
-        self.build_paths = []
+        self.build_paths: list[Path] = []
         self.workspace = workspace
-        self.makex_file_checksum = checksum
         self.makex_file = makex_file or None
 
+        self._include_function = include_function
+        self._globals: dict[str, Any] = globals or {}
+        self.macros: dict[str, Callable] = {} if macros is None else macros
+        self.block_registration = False
+        self.includes: set[MakexFile] = set()
+
     def globals(self):
+        parent = super().globals()
+
         g = {
+            #**self._globals,
+            **parent,
+            TARGETS_MODULE_VARIABLE: self.targets,
+            MACROS_MODULE_VARIABLE: self.macros,
             "Environment": self.environment, #"pattern": wrap_script_function(self._pattern),
+            "ENVIRONMENT": self.environment,
             "target": wrap_script_function(self._function_target),
-            "Target": wrap_script_function(self._function_Target),
+
+ # TODO: declare new aliases:
+            "Task": wrap_script_function(self._function_task),
+            "task": wrap_script_function(self._function_task),
+            _TARGET_REFERENCE_NAME: wrap_script_function(self._function_Target),
+            #TODO: define a Target object for type references
+            #"Target": wrap_script_function(self._function_Target),
+            _MACRO_DECORATOR_NAME: self._decorator_macro, #"macro": Decorator,
         }
+
+        if INCLUDE_ENABLED:
+            g["include"] = self._function_include
+
         # path utilities
         g.update(
             {
-                "path": wrap_script_function(self._function_path),
-                # TODO: path() is a common variable (e.g. in a loop), and as an argument (to target) and Path() object. confusing.
+                # DONE: path() is a common variable (e.g. in a loop), and as an argument (to target) and Path() object. confusing.
                 #  alias to cache(), or output()
-                #"cache": wrap_script_function(self.build_path),
+                "path": wrap_script_function(self._function_path),
+                "task_path": wrap_script_function(self._function_task_path),
+                # cache is a bit shorter than task_path
+                "cache": wrap_script_function(self._function_task_path),
                 #"output": wrap_script_function(self.build_path),
                 "Path": wrap_script_function(self._function_Path),
                 "source": wrap_script_function(self._function_source),
             }
         )
 
         if GLOB_FUNCTION_ENABLED:
             g["glob"] = wrap_script_function(self._function_glob)
 
         if FIND_FUNCTION_ENABLED:
             g["find"] = wrap_script_function(self._function_find)
 
-        # runnables
+        # Actions
         g.update(
             {
                 "print": wrap_script_function(self._function_print),
                 "shell": wrap_script_function(self._function_shell),
+                # TODO: deprecate sync
                 "sync": wrap_script_function(self._function_sync),
+                "mirror": wrap_script_function(self._function_sync),
                 "execute": wrap_script_function(self._function_execute),
                 "copy": wrap_script_function(self._function_copy),
                 "write": wrap_script_function(self._function_write),
                 "environment": wrap_script_function(self._function_environment),
             }
         )
 
@@ -1982,25 +1759,115 @@
         if EXPAND_FUNCTION_ENABLED:
             g["expand"] = wrap_script_function(self._function_expand)
 
         if HOME_FUNCTION_ENABLED:
             g["home"] = wrap_script_function(self._function_home)
         return g
 
+    @dataclass
+    class MacroContext:
+        target: Callable
+        path: Callable
+        source: Callable
+
+    def _decorator_macro(self, fn, _location1_=None):
+        # @macro decorator implementation
+        # wrap functions to handle location argument
+        # TODO: macros should be keyword only.
+        def f(
+            *args,
+            _location_=None,
+            **kwargs,
+        ):
+            if args:
+                raise PythonScriptError("Macros must be called with keyword arguments.", _location_)
+
+            debug("Calling macro %s %s %s %s", fn, args, kwargs, _location_)
+            return fn(*args, **kwargs)
+
+        trace(f"Declaring macro: %s: %s (%s)", self.path, fn.__name__, _location1_)
+        self.macros[fn.__name__] = f
+        f.__name__ = fn.__name__
+
+        # slighly similar way to achieve the same goal:
+        #self._globals[fn.__name__] = f
+        #import inspect
+        #inspect.stack()[1][0].f_globals.update()
+        return f
+
+    if False:
+
+        def has_global(self, name):
+            print("check has global", name)
+            return name in self._globals
+
+        def get_global(self, name):
+            return self._globals.get(name)
+
+    def _function_include(
+        self,
+        path: StringValue,
+        search=False,
+        tasks=False,
+        _globals=None,
+        required=True,
+        _location_=None,
+        **kwargs
+    ):
+
+        # _globals argument is passed in via ast modifications
+        if self._include_function is None:
+            raise PythonScriptError("Can't include from this file.", _location_)
+
+        debug("Including %s ...", path)
+        module, file = self._include_function(
+            ctx=self.ctx,
+            workspace=self.workspace,
+            base=self.directory,
+            makex_file=self.makex_file,
+            search_path=path,
+            search=search,
+            globals=_globals,
+            location=_location_,
+            targets=tasks,
+            required=required,
+            extra=kwargs,
+        )
+
+        if module is None:
+            debug("Skipping missing optional makex file.")
+            return None
+
+        del module.__builtins__
+        _macros = getattr(module, MACROS_MODULE_VARIABLE)
+        debug("Importing macros from %s: %s", path, _macros.keys())
+
+        _globals.update(_macros)
+
+        self.includes.add(file)
+
+        if tasks:
+            trace("Adding targets from included file: %s", module._TARGETS_.keys())
+            self.targets.update(module._TARGETS_)
+
     def _function_expand(self, string: StringValue, location: FileLocation):
         return Expansion(context=self.ctx, string=string, location=location)
 
-    def _function_home(self, user=None, location=None):
+    def _function_home(self, *path, user=None, location=None):
         if user:
             arg = f"~{user}"
         else:
             arg = "~"
         home = expanduser(arg)
 
-        return PathElement(arg, resolved=Path(home), location=location)
+        _path = Path(home)
+        if path:
+            _path =  _path.joinpath(*path)
+
+        return PathElement(arg, resolved=_path, location=location)
 
     def _function_find(
         self, path: PathLikeTypes, expr: Union[Glob, RegularExpression] = None, location=None
     ):
 
         if isinstance(path, StringValue):
             _path = resolve_string_path_workspace(self.ctx, self.workspace, path, self.directory)
@@ -2013,82 +1880,89 @@
                 f"Invalid path type in find() function: {type(path)} ({path}). Path or string expected.",
                 location
             )
         return FindFiles(expr, path, location=location)
 
     def _function_environment(
         self,
-        dictionary: Mapping[StringValue, Union[PathLikeTypes, StringValue]] = None,
+        dictionary: Optional[dict[StringValue, Union[PathLikeTypes, StringValue]]] = None,
         location: FileLocation = None,
         **kwargs: Union[PathLikeTypes, StringValue],
     ):
-        dictionary = dictionary or {}
-        dictionary.update(**kwargs)
-        return SetEnvironment(dictionary, location=location)
+        _dictionary = dictionary or {}
+        _dictionary.update(**kwargs)
+        return SetEnvironment(_dictionary, location=location)
 
     def _function_Target(self, name, path: PathLikeTypes = None, location=None, **kwargs):
         # absorb kwargs so we can error between Target and target
         return TargetReferenceElement(name=name, path=path, location=location)
 
     def _function_path(
         self,
+        *args,
+        **kwargs,
+    ):
+        location = kwargs.get("location", "")
+
+        self.ctx.ui.warn(
+            f"The path() function is deprecated. Please change to using task_path() instead. {location}"
+        )
+        return self._function_task_path(*args, **kwargs)
+
+    def _function_task_path(
+        self,
         name,
         path: PathLikeTypes = None,
-        variants: list[str] = None,
+        variants: Optional[list[str]] = None,
         location=None,
     ):
         if isinstance(path, PathElement):
             _path = resolve_path_element_workspace(self.ctx, self.workspace, path, self.directory)
         elif isinstance(path, StringValue):
             _path = resolve_string_path_workspace(self.ctx, self.workspace, path, self.directory)
         elif path is None:
             _path = self.directory
         else:
             raise PythonScriptError(f"Invalid path value:{type(path)}", location)
-
         return create_build_path_object(
             self.ctx, target=name, path=_path, variants=variants, location=location
         )
 
     def _function_source(self, *path: StringValue, location=None):
         if not path:
             # XXX: No path. Return the source directory.
             return PathElement(*self.directory.parts, resolved=self.directory, location=location)
 
-        #parts = []
         for part in path:
             if not isinstance(part, StringValue):
                 raise PythonScriptError(
                     f"Invalid path part type in source() function. Expected string. Got {type(part)}: {part!r}",
                     getattr(part, "location", location)
                 )
 
-        #_path = resolve_path_parts(parts, self.directory, location)
         _path = resolve_path_parts_workspace(
             self.ctx, self.workspace, path, self.directory, location
         )
 
         # XXX: all of _path.parts is used, so it's fully absolute
         return PathElement(*path, resolved=_path, location=location)
 
-    def _function_Path(self, *path: PathLikeTypes, location=None):
-        #parts = []
+    def _function_Path(self, *path: StringValue, location=None):
         for part in path:
             if not isinstance(part, StringValue):
                 raise PythonScriptError(
                     f"Invalid path part type in Path() function. Expected string. Got {type(part)}: {part!r}",
                     getattr(part, "location", location)
                 )
 
-        trace("Creating path: %s", path)
-        #_path = resolve_path_parts(parts, self.directory, location)
-
+        #trace("Creating path: %s", path)
         if True:
             _path = None
         else:
+            # TODO: handle resolving workspace paths here
             _path = resolve_path_parts_workspace(
                 self.ctx, self.workspace, path, self.directory, location
             )
 
         return PathElement(*path, resolved=_path, location=location)
 
     def _function_archive(self, path: PathLikeTypes = None, *, prefix=None, location=None):
@@ -2098,52 +1972,58 @@
         for part in script:
             if not isinstance(part, StringValue):
                 raise PythonScriptError(
                     f"Invalid script in shell function. Expected string. Got {type(part)}: {part!r}",
                     getattr(part, "location", location)
                 )
 
-        return ShellCommand(script, location)
+        return Shell(script, location)
 
     def _function_execute(
         self,
         file: PathLikeTypes,
         /,
         *args: Union[tuple[PathLikeTypes], tuple[PathLikeTypes, ...]],
         **kwargs, #environment: dict[str, str] = None,
         #location=None,
     ):
-        environment = kwargs.get("environment", None)
+        environment = kwargs.pop("environment", None)
+        location = kwargs.pop("location", None)
 
         if isinstance(file, ListTypes):
             file = file[0]
             args = file[1:]
         return Execute(
             file,
             args,
             environment=environment,
-            location=kwargs.get("location", None),
+            location=location,
         )
 
     def _function_glob(self, glob: str, location=None):
         return Glob(glob, location)
 
     def _function_print(self, *messages, location=None):
         return Print(messages, location)
 
-    def _function_write(self, destination: PathLikeTypes, data: StringValue = None, location=None):
+    def _function_write(
+        self,
+        destination: PathLikeTypes,
+        data: StringValue = None,
+        executable=False,
+        location=None
+    ):
         # contents=None for touch
-        return Write(destination, data=data, location=location)
+        return Write(destination, data=data, executable=executable, location=location)
 
     def _function_sync(
         self, source: list[AllPathLike], destination: PathLikeTypes = None, /, **kwargs
     ):
         location: FileLocation = kwargs.pop("location", None)
         exclude: list[Union[StringValue, Glob]] = kwargs.pop("exclude", None)
-        destination: PathLikeTypes = destination
         return Synchronize(
             source=source,
             destination=destination,
             exclude=exclude,
             location=location,
         )
 
@@ -2162,15 +2042,15 @@
             location=location,
         )
 
     def _target_requires(
         self,
         requirements: list[Union[PathElement, StringValue, Glob, TargetReferenceElement]],
         location,
-    ) -> Iterable[Union[TargetReferenceElement, PathElement, Glob]]:
+    ) -> Iterable[Union[TargetReferenceElement, PathElement, Glob, FindFiles]]:
         # process the requires= list of the target() function.
         # convert to TargetReference where appropriate
         for require in requirements:
             if isinstance(require, StringValue):
                 if require.value.find(":") >= 0:
                     # abbreviated target reference as a string
                     rpath, target = require.value.split(":")
@@ -2197,66 +2077,118 @@
                     # convert strings to paths
                     p = resolve_string_path_workspace(
                         self.ctx, self.workspace, require, self.directory
                     )
                     yield PathElement(require, resolved=p, location=require.location)
 
             elif isinstance(require, TargetReferenceElement):
-                # append internal objects referring to files such as is find(), glob() and Target(); these will be expanded later
+                # append references which will be evaluated later
                 yield require
             elif isinstance(require, FindFiles):
                 # append internal objects referring to files such as is find(), glob() and Target(); these will be expanded later
                 if FIND_IN_INPUTS_ENABLED is False:
                     raise PythonScriptError(
                         "The find function (find()) is not allowed in the target's requires list.",
                         require.location
                     )
 
                 yield require
             elif isinstance(require, Glob):
+                # append internal objects referring to files such as is find(), glob() and Target(); these will be expanded later
                 if GLOBS_IN_INPUTS_ENABLED is False:
                     raise PythonScriptError(
                         "The glob function (glob) is not allowed in the target's requires list.",
                         require.location
                     )
-                # append internal objects referring to files such as is find(), glob() and Target(); these will be expanded later
                 yield require
             elif isinstance(require, PathElement):
                 yield require
             elif isinstance(require, TargetObject):
                 raise PythonScriptError("Invalid use of target() for the requires args. ", location)
             elif isinstance(require, ListTypes):
                 # TODO: wrap lists so we can get a precise location.
                 # TODO: limit list depth.
                 yield from self._target_requires(require, location)
             else:
                 raise PythonScriptError(
                     f"Invalid type {type(require)} in requires list. Got {require!r}.", location
                 )
 
+    class TargetArguments(TypedDict):
+        name: str
+        path: NotRequired[Path]
+        requires: NotRequired[list[str]]
+        runs: NotRequired[list]
+        actions: NotRequired[list]
+        outputs: NotRequired[list]
+        inputs: NotRequired[dict]
+        location: Required[FileLocation]
+        #**kwargs: Unpack[TargetArguments]
+        # NotRequired
+        #
+
     def _function_target(
-        self,
-        name,
-        *,
-        path=None,
-        requires=None,
-        runs=None,
-        outputs=None,
-        location: FileLocation = None,
+        self, #*args,
+        **kwargs: Unpack[TargetArguments],
     ):
+        location = kwargs.get("location", None)
+        self.ctx.ui.warn(
+            f"The target() function is deprecated. It will be removed by 2024-06. Please change to using task(steps=[]) instead. {location}"
+        )
+        steps = kwargs.pop("runs", None)
+        return self._function_task(steps=steps, **kwargs)
+
+    def _function_task(
+        self, #*args,
+        **kwargs: Unpack[TargetArguments],
+    ):
+        location = kwargs.pop("location", None)
+
+        if False:
+            arglen = len(args)
+            if not arglen:
+                pass
+            elif arglen == 3:
+                name, path, variants = args
+                return TargetReferenceElement(name, path, variants, location=location)
+            elif arglen == 2:
+                name, path = args
+                return TargetReferenceElement(name, path, location=location)
+            elif arglen == 1:
+                name = args[0]
+                return TargetReferenceElement(name, location=location)
+            else:
+                raise PythonScriptError(
+                    "Invalid number of arguments to create Target Reference. Expected name and optional path.",
+                    location=location
+                )
+
+        if self.block_registration:
+            trace("Registration of target blocked at %s", location)
+            return
+
+        #trace("Calling target() from %s", self.makex_file)
+        name = kwargs.pop("name", None)
+        path = kwargs.pop("path", None)
+        requires = kwargs.pop("requires", None)
+        runs = kwargs.pop("actions", None) or kwargs.pop("steps", None)
+        outputs = kwargs.pop("outputs", None)
+
+        if kwargs:
+            raise PythonScriptError(f"Unknown arguments to task(): {kwargs}", location)
 
         if name is None or name == "":
             raise PythonScriptError(f"Invalid target name {name!r}.", location)
 
         _validate_target_name(name, getattr(name, "location", location))
 
         existing: TargetObject = self.targets.get(name, None)
         if existing:
             raise PythonScriptError(
-                f"Duplicate target name {name!r}. Already defined at {existing.location.path}:{existing.location.line}.",
+                f"Duplicate target name {name!r}. Already defined at {existing.location}.",
                 location
             )
 
         if requires:
             _requires = list(self._target_requires(requires, location))
         else:
             _requires = []
@@ -2264,525 +2196,247 @@
         _outputs = []
 
         # unnamed outputs go in None
         outputs_dict = {None: []}
         unnamed_outputs = outputs_dict.get(None)
 
         if outputs:
-
-            def process_output(
-                output: Union[StringValue, Glob],
-                location,
-            ) -> Union[PathElement, PathObject, Glob]:
-                # Mostly return the outputs, as is, for later evaluation. Check for invalid arguments early.
-                if isinstance(output, StringValue):
-                    return PathElement(output, location=output.location)
-                elif isinstance(output, Glob):
-                    # append glob as is. we'll resolve later.
-                    return output
-                elif isinstance(output, PathObject):
-                    return output
-                elif isinstance(output, PathElement):
-                    return output
-                else:
-                    raise PythonScriptError(
-                        f"Invalid output type {type(output)} in output list for target {name}: {output}",
-                        location
-                    )
-
             if isinstance(outputs, ListTypes):
-                for out in outputs:
-                    output = process_output(out, location)
+                for i, out in enumerate(outputs):
+                    output = _process_output(out, name, location)
                     _outputs.append(output)
                     unnamed_outputs.append(output)
+                    outputs_dict[i] = output
 
             elif NAMED_OUTPUTS_ENABLED and isinstance(outputs, dict):
                 # named outputs
                 for k, v in outputs.items():
-                    output = process_output(v, location)
+                    output = _process_output(v, name, location)
                     _outputs.append(output)
                     outputs_dict[k] = output
             else:
                 raise PythonScriptError(
                     f"Invalid outputs type {type(outputs)}. Should be a list.", location
                 )
 
+        if TARGET_PATH_ENABLED is False and path is not None:
+            raise PythonScriptError(
+                "Setting path is not allowed (by flag). TARGET_PATH_ENABLED",
+                getattr(path, "location", location)
+            )
+
         target = TargetObject(
             name=name,
             path=path,
             requires=_requires,
             run=runs or [], # commands will be evaluated later
             outputs=_outputs,
             outputs_dict=outputs_dict,
             workspace=self.workspace,
             makex_file=self.makex_file,
             location=location,
         )
+
         self.targets[name] = target
+        trace("Registered target %s in makexfile %s. %s ", target.name, self.makex_file, location)
         return None
 
 
 class MakexFile:
     # to the makefile
     path: Path
 
     targets: dict[str, TargetObject]
 
+    macros: dict[str, Callable]
+
+    code: Optional[types.CodeType] = None
+
     def __init__(self, ctx, path: Path, targets=None, variables=None, checksum: str = None):
         self.ctx = ctx
         self.path = path
         self.directory = path.parent
         self.targets = targets or {}
         self.variables = variables or []
         self.checksum = checksum
-        self.enviroment_hash = None
+        self.environment_hash = None
+        self.macros = {}
+
+        # list of paths this MakexFile imports or includes.
+        # TODO: Must be included in hash.
+        self.includes: list[MakexFile] = []
+
+    def hash_components(self):
+        yield f"version:{VERSION}"
+        yield f"environment:{self.environment_hash}"
+        yield f"makex-file:{self.checksum}"
+        for include in self.includes:
+            yield f"environment:include:{include.environment_hash}"
+            yield f"makex-file:include:{include.checksum}"
 
     def key(self):
         return str(self.path)
 
     @classmethod
-    def parse(cls, ctx: Context, path: Path, workspace: Workspace) -> "MakexFile":
-        debug("Started parsing makefile %s ...", path)
-
+    def preparse(cls, ctx: Context, path: Path, workspace: Workspace, include_function) -> ast.AST:
+        trace("PREPARSE %s", path)
         checksum = FileChecksum.create(path)
         checksum_str = str(checksum)
-
         makefile = cls(ctx, path, checksum=checksum_str)
-
-        env = MakefileScriptEnv(
+        env = MakexFileScriptEnvironment(
             ctx,
             directory=path.parent,
             path=path,
             makex_file=makefile,
             targets=makefile.targets,
+            macros=makefile.macros,
             workspace=workspace,
-            checksum=checksum_str,
+            include_function=include_function
         )
 
         _globals = {}
 
         # add environment variables to makefiles as variables
         if ENVIRONMENT_VARIABLES_IN_GLOBALS_ENABLED:
             _globals.update(ctx.environment)
 
-        script = PythonScriptFile(path, env, _globals)
-
-        with path.open("rb") as f:
-            script.execute(f)
+        posix_path = path.as_posix()
+        include_processor = ProcessIncludes(posix_path)
 
-        if HASH_USED_ENVIRONMENT_VARIABLES:
-            # hash the enviroment variable usages so targets change when they change.
-            usages = env.environment._usages()
-            if usages:
-                makefile.enviroment_hash = target_hash(
-                    "".join(f"{k}={v}" for k, v in sorted(usages.items()))
-                )
-
-        debug("Finished parsing makefile %s.", path)
-        return makefile
-
-
-class ParseResult:
-    makex_file: MakexFile = None
-    errors: deque[PythonScriptError]
-
-    def __init__(self, makex_file=None, errors=None):
-        self.errors = errors
-        self.makex_file = makex_file
-
-
-def parse_makefile_into_graph(
-    ctx: Context,
-    path: Path,
-    graph: TargetGraph,
-    threads=2,
-    allow_makex_files=DIRECT_REFERENCES_TO_MAKEX_FILES,
-) -> ParseResult:
-    assert ctx.workspace_object
-
-    # link from path -> path so we can detect cycles
-    linkages: dict[ResolvedTargetReference, list[ResolvedTargetReference]] = {}
-
-    # set this event to stop the parsing loop
-    stop = Event()
-
-    # any errors collected during parsing
-    errors = deque()
-
-    # any makefiles completed (either success or error)
-    completed: deque[Path] = deque()
-
-    # paths added to thread pool ready to parse
-    executing: deque[Path] = deque()
-
-    # waiting to be queued for work; requirements added from other files
-    input_queue: deque[Path] = deque([path])
-
-    _initial = path
-    _finished: dict[Path, MakexFile] = {}
-
-    def stop_and_error(error):
-        stop.set()
-        errors.append(error)
-
-    def _iterate_target_requires(
-        makefile_path: Path,
-        makefile: MakexFile,
-        target: TargetObject,
-    ) -> Iterable[ResolvedTargetReference]:
-        # yields a list of Paths the specified makefile requires
-        #debug("Check requires %s -> %s", target, target.requires)
-        #target_input = makefile.directory
-        target_input = target.path_input()
-        workspace = target.workspace
-
-        assert isinstance(workspace, Workspace)
-
-        for require in target.requires:
-            trace("Process requirement %s", require)
-            if isinstance(require, TargetObject):
-                # we have a Target object.
-                # TODO: This is used in testing. Not really important.
-                # Manually constructed target objects.
-                trace("Yield target", require)
-                makex_file = require.makex_file_path
-                yield ResolvedTargetReference(
-                    require.name, Path(makex_file), location=require.location
-                )
-
-            elif isinstance(require, TargetReferenceElement):
-                name = require.name
-                path = require.path
+        script = PythonScriptFile(
+            path, _globals, extra_visitors=[TransformGetItem(posix_path), include_processor]
+        )
+        script.set_disabled_assignment_names(DISABLE_ASSIGNMENT_NAMES)
 
-                if isinstance(path, StringValue):
-                    # Target(name, "path/to/target")
-                    #trace("Path is string value: %r", path)
-                    search_path = resolve_string_path_workspace(
-                        ctx, target.workspace, path, target_input
-                    )
+        with path.open("rb") as f:
+            return script.parse(f)
 
-                    trace("Resolve search path from string %r: %s", path, search_path)
-                    # we could have a directory, or we could have a file
-                    if search_path.is_file():
-                        if allow_makex_files:
-                            yield ResolvedTargetReference(name, search_path, path.location)
-                            continue
-                        else:
-                            error = ExecutionError(
-                                "References directly to makex files are not allowed."
-                                " Strip the makex file name.",
-                                target,
-                                path.location
-                            )
-                            stop_and_error(error)
-                            raise error
-                    #trace("Searching path for makex files: %s", search_path)
-                    makex_file = find_makex_files(search_path, ctx.makex_file_names)
-
-                    trace("Resolved makex file from string %s: %s", path, makex_file)
-                    if makex_file is None:
-                        error = ExecutionError(
-                            f"No makex files found in path {search_path} {path!r} for the target's requirements."
-                            f" Tried: {ctx.makex_file_names!r} {target}",
-                            target,
-                            path.location
-                        )
-                        stop_and_error(error)
-                        raise error
-                    yield ResolvedTargetReference(name, makex_file, path.location)
-                elif isinstance(path, PathElement):
-                    # allow users to specify an absolute path to
-                    # Target(name, Path("path/to/something")))
-                    search_path = resolve_path_element_workspace(
-                        ctx, target.workspace, path, target_input
-                    )
-                    trace("Resolve search path from %r: %s", path, search_path)
+    @classmethod
+    def execute(
+        cls,
+        ctx: Context,
+        path: Path,
+        workspace: Workspace,
+        node: ast.AST,
+        include_function,
+        globals=None,
+        importer=None
+    ) -> "MakexFile":
+        pass
 
-                    # we could have a directory, or we could have a file
-                    if search_path.is_file():
+    @classmethod
+    def parse(
+        cls,
+        ctx: Context,
+        path: Path,
+        workspace: Workspace,
+        include_function,
+        globals=None,
+        importer=None
+    ) -> "MakexFile":
+        """
+
+        Globals may be passed in for uses such as include(). Globals dictionary shall contain task() and other defined functions.
+        When task is called in an included file, the task should register the including file. It's hacky, but it works.
+
+        :param ctx:
+        :param path:
+        :param workspace:
+        :param include_function:
+        :param globals:
+        :param importer:
+        :return:
+        """
+        debug("Started parsing makefile %s ...", path)
 
-                        if allow_makex_files:
-                            yield ResolvedTargetReference(name, search_path, path.location)
-                            continue
-                        else:
-                            error = ExecutionError(
-                                "References directly to makex files are not allowed. Strip the makex file name.",
-                                target,
-                                path.location
-                            )
-                            stop_and_error(error)
-                            raise error
-                            break
-
-                    makex_file = find_makex_files(search_path, ctx.makex_file_names)
-
-                    trace("Resolved makex file from pathelement %s: %s", path, makex_file)
-                    if makex_file is None:
-                        error = ExecutionError(
-                            f"No makex files found in path {search_path} for the target's requirements.",
-                            target,
-                            path.location
-                        )
-                        stop_and_error(error)
-                        raise error
+        checksum = FileChecksum.create(path)
+        checksum_str = str(checksum)
 
-                    yield ResolvedTargetReference(name, makex_file, path.location)
-                elif path is None:
-                    # Target(name)
-                    # we're referring to this file. we don't need to parse anything.
-                    yield ResolvedTargetReference(name, makefile_path, require.location)
-                else:
-                    debug("Invalid ref type %s: %r", type(path), path)
-                    exc = Exception(f"Invalid reference path type {type(path)}: {path!r}")
-                    stop_and_error(exc)
-                    raise exc
-                #debug("Got reference %s %s", name, path)
-                #l.append(ResolvedTargetReference(name, path))
-
-    def finished(makefile_path: Path, makefile: Future[MakexFile]):
-        makefile_path = Path(makefile_path)
-        trace("Makefile parsing finished in thread %s: %s", current_thread().ident, makefile_path)
-
-        e = makefile.exception()
-        if e:
-            if not isinstance(e, (ExecutionError, PythonScriptError)):
-                logging.error("Makefile had an error %s %r", e, e)
-                logging.exception(e)
+        # TODO: this needs to be refactored. we should create the makefile last.
+        makefile = cls(ctx, path, checksum=checksum_str)
 
-            errors.append(e)
+        env = MakexFileScriptEnvironment(
+            ctx,
+            directory=path.parent,
+            path=path,
+            makex_file=makefile,
+            targets=makefile.targets,
+            macros=makefile.macros,
+            workspace=workspace,
+            include_function=include_function
+        )
 
-            mark_path_finished(makefile_path)
-            return
+        # reuse the globals, except for the one that defines a macro
+        # we want the target() and path() functions to work as they would in the includer.
+        # path should resolve relative to includer
+        # target() should be registered in includer
 
-        makefile = makefile.result()
+        if globals:
+            _globals = {"FILE": path, **env.globals(), **globals}
+        else:
+            _globals = {"FILE": path, **env.globals()}
 
-        _finished[makefile_path] = makefile
+        # force the use of the local environments macro decorator, ignoring anything passed in
+        _globals[_MACRO_DECORATOR_NAME] = env._decorator_macro
 
-        if makefile.targets:
-            trace(
-                "Adding %d targets from makefile...",
-                len(makefile.targets), #makefile.targets[:min(3, len(makefile.targets))]
-            )
+        #debug("Globals before parse %s %s", path, _globals)
 
-            # we're done. add the target references to the parsing input queue
-            for target_name, target in makefile.targets.items():
-                trace("Add target to graph %s %s ", target, target.key())
-                try:
-                    graph.add_target(ctx, target)
-                except ExecutionError as e:
-                    errors.append(e)
-                    mark_path_finished(makefile_path)
-                    return
+        # add environment variables to makefiles as variables
+        if ENVIRONMENT_VARIABLES_IN_GLOBALS_ENABLED:
+            _globals.update(ctx.environment)
 
-                t_as_ref = ResolvedTargetReference(
-                    target.name, Path(target.makex_file_path), target.location
-                )
+        posix_path = path.as_posix()
+        if INCLUDE_ENABLED:
+            include_processor = ProcessIncludes(posix_path)
+        else:
+            include_processor = None
+
+        script = PythonScriptFile(
+            path,
+            _globals,
+            importer=importer,
+            pre_visitors=[include_processor] if INCLUDE_ENABLED else [],
+            extra_visitors=[TransformGetItem(posix_path)],
+            enable_imports=IMPORT_ENABLED,
+        )
+        script.set_disabled_assignment_names(DISABLE_ASSIGNMENT_NAMES)
 
-                trace("Check requires %s -> %r", target.key(), target.requires)
+        # TODO: parse the file, find any includes, parse those and insert their asts before we execute.
+        with path.open("rb") as f:
+            tree = script.parse(f)
 
-                # TODO: store this iteration for later (target evaluation in Executor)
-                #  we're duplicating code there.
-                iterable = _iterate_target_requires(
-                    makefile=makefile,
-                    makefile_path=makefile_path,
-                    target=target,
+        if False and INCLUDE_ENABLED:
+            asts = []
+            for search_path, location in include_processor.includes_seen:
+                trace("AST INCLUDE: %s", search_path)
+                asts += include_function(
+                    ctx, workspace, path.parent, search_path, location, search=True
                 )
-                for reference in iterable:
-                    # Check for any cycles BETWEEN files and targets.
-                    cycles = linkages.get(reference, None)
-                    #trace("Linkages of %s: %s", reference, cycles)
-                    linkages.setdefault(t_as_ref, list()).append(reference)
-                    if cycles and (t_as_ref in cycles):
-                        mark_path_finished(makefile_path)
-                        error = MakexFileCycleError(
-                            f"Cycle detected from {reference.key()} to {cycles[-1].key()}",
-                            target,
-                            cycles,
-                        )
-                        errors.append(error)
-                        raise error
-
-                    #trace("Got required path %s", reference)
-                    if reference.path in completed:
-                        trace("Path already completed %s. Possible cycle.", reference)
-                        continue
-
-                    trace("Add to parsing input queue %s", reference)
-                    input_queue.append(reference.path)
-                    target.add_resolved_requirement(reference)
 
-        #if path in queued:
-        trace("Remove from deque %s", makefile_path)
-        mark_path_finished(makefile_path)
+            InsertAST(path, asts).visit(tree)
 
-    def mark_path_finished(makefile_path: Path):
-        completed.append(makefile_path)
+        makefile.macros = env.macros
 
-        if makefile_path in executing:
-            executing.remove(makefile_path)
+        # store a code object so we can reuse it
+        makefile.code = script.execute(tree)
 
-    pool = ThreadPoolExecutor(threads)
+        makefile.includes.extend(env.includes)
 
-    try:
-        while stop.is_set() is False:
-
-            if len(input_queue) == 0:
-                debug("Stopped. Empty queue.")
-                stop.set()
-                continue
-
-            while len(executing) == threads:
-                debug("queue wait. %s", executing)
-                time.sleep(1)
-
-            path = input_queue.pop()
-
-            if path in executing:
-                input_queue.append(path)
-            else:
-                if path not in completed:
-                    if NESTED_WORKSPACES_ENABLED:
-                        workspace_of_makefile: Workspace = ctx.workspace_cache.get_workspace_of(
-                            path
-                        )
-                        trace(
-                            "Detected workspace of makefile at path %s: %s",
-                            path,
-                            workspace_of_makefile
-                        )
-                    else:
-                        # Use the root/initial workspace if no nesting.
-                        workspace_of_makefile = ctx.workspace_object
-
-                    debug(
-                        "Queue MakeFile for parsing %s (workspace=%s) ...",
-                        path,
-                        workspace_of_makefile
-                    )
-
-                    f = pool.submit(
-                        MakexFile.parse,
-                        ctx=ctx,
-                        path=Path(path),
-                        workspace=workspace_of_makefile,
-                    )
-                    # We must use a lambda passing the path because if we have
-                    #  an Exception we won't know which file caused it.
-                    f.add_done_callback(lambda future, p=path: finished(p, future))
-
-                    executing.append(path)
-                    input_queue.append(path)
-                    # XXX: this sleep is required so that is_set isn't called repeatedly (thousands of times+) when running.
-                    time.sleep(0.1)
-
-    finally:
-        debug("Wait for pool to shutdown...")
-        pool.shutdown()
-
-    return ParseResult(makex_file=_finished.get(_initial), errors=errors)
-
-
-def parse_target_string_reference(
-    ctx: Context,
-    base,
-    string,
-    check=True,
-) -> Optional[ResolvedTargetReference]:
-    # resolve the path/makefile?:target_or_build_path name
-    # return name/Path
-    parts = string.split(":", 1)
-    if len(parts) == 2:
-        path, target = parts
-        path = Path(path)
-        if not path.is_absolute():
-            path = base / path
+        if HASH_USED_ENVIRONMENT_VARIABLES:
+            # hash the environment variable usages so targets change when they change.
+            usages = env.environment._usages()
+            if usages:
+                makefile.environment_hash = target_hash(
+                    "".join(f"{k}={v}" for k, v in sorted(usages.items()))
+                )
 
-        if path.is_symlink():
-            path = path.readlink()
-    else:
-        target = parts[0]
-        path = base
+        debug(
+            "Finished parsing makefile %s: Macros: %s | Targets: %s",
+            path,
+            makefile.macros.keys(),
+            _globals[TARGETS_MODULE_VARIABLE].keys()
+        )
+        makefile.targets = _globals[TARGETS_MODULE_VARIABLE]
+        return makefile
 
-    if path.is_dir():
-        if check:
-            # check for Build/Makexfile in path
-            path, checked = find_makex_files(path, ctx.makex_file_names)
-            if path is None:
-                ctx.ui.print(
-                    f"Makex file does not exist for target specified: {target}", error=True
-                )
-                for check in checked:
-                    ctx.ui.print(f"- Checked in {check}")
-                sys.exit(-1)
-
-    return ResolvedTargetReference(target, path=path)
-
-
-#def _string_value_to_path(ctx, base, value: StringValue) -> Path:
-#    val = value.value
-#
-#    if False and val.startswith("~"):
-#        # TODO: use environment HOME to expand the user
-#        return Path(val).expanduser()
-#    else:
-#        path = Path(val)
-#
-#        if not path.is_absolute():
-#            path = base / path
-#
-#        return path
-
-#def _path_element_to_path(base, value: PathElement) -> Path:
-#    return resolve_path_element(value, base)
-#    if value.resolved:
-#        source = value.resolved
-#        if not source.is_absolute():
-#            source = base / source
-#    else:
-#        source = value._as_path()
-#        #source = source.expanduser()
-#        if not source.is_absolute():
-#            source = base / source
-#
-#    return source
-#def resolve_path_element(element: PathElement, base: Path) -> Path:
-#    """
-#    Resolve an unresolved relative PathObject.
-#
-#    :param element:
-#    :param base:
-#    :return:
-#    """
-#
-#    #if search_path.parts[0] == "//":
-#    #    error = NotImplementedError("Workspace paths not supported yet.")
-#    #    stop_and_error(error)
-#    #    break
-#
-#    if element.resolved:
-#        return element.resolved
-#
-#    path = Path(*element.parts)
-#
-#    if not path.is_absolute():
-#        path = base / path
-#    return path
-
-#def resolve_path_parts(parts: list[StringValue], base: Path, location) -> Path:
-#    path = Path(*parts)
-#
-#    _validate_path(path.parts, location)
-#
-#    if not path.is_absolute():
-#        path = base / path
-#
-#    return path
-
-#def resolve_string_path(element: StringValue, base: Path) -> Path:
-#    path = Path(element.value)
-#
-#    _validate_path(path.parts, element.location)
-#
-#    if not path.is_absolute():
-#        path = base / path
-#
-#    return path
+    def __repr__(self):
+        return self.key()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `makex-20240203/python/makex/makefile_test.py` & `makex-20240401/python/makex/makex_file_parser_test.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from pathlib import Path
 
+import pytest
 from makex.context import Context
 from makex.errors import ExecutionError
-from makex.make_file import (
-    MakexFileCycleError,
-    ResolvedTargetReference,
+from makex.makex_file import MakexFileCycleError
+from makex.makex_file_parser import (
     TargetGraph,
     parse_makefile_into_graph,
 )
+from makex.makex_file_types import ResolvedTargetReference
 from makex.python_script import PythonScriptError
 from makex.workspace import Workspace
 
 
 def test_parse(tmp_path: Path):
     """
     Test parsing of targets.
     """
     a = tmp_path / "Makexfile"
-    a.write_text("""target(name="a")""")
+    a.write_text("""task(name="a")""")
 
     ctx = Context()
     ctx.workspace_object = Workspace(tmp_path)
     graph = TargetGraph()
     result = parse_makefile_into_graph(ctx, a, graph)
     assert not result.errors
     assert ResolvedTargetReference("a", a) in graph
@@ -32,17 +33,17 @@
     Test the parsing of a target requiring a target in another path.
     """
     a = tmp_path / "Makexfile"
     b = tmp_path / "sub" / "Makexfile"
 
     b.parent.mkdir(parents=True)
 
-    a.write_text("""target(name="a",requires=[Target("b", "sub")])""")
+    a.write_text("""task(name="a",requires=[Reference("b", "sub")])""")
 
-    b.write_text("""target(name="b")""")
+    b.write_text("""task(name="b")""")
 
     ctx = Context()
     ctx.workspace_object = Workspace(tmp_path)
     graph = TargetGraph()
     result = parse_makefile_into_graph(ctx, a, graph)
 
     assert not result.errors
@@ -52,18 +53,18 @@
 
 
 def test_cycle_error_external_targets(tmp_path: Path):
     """
     Test cycles between targets of different files.
     """
     makefile_path_a = tmp_path / "Makexfile-a"
-    makefile_path_a.write_text("""target(name="a",requires=["Makexfile-b:b"])\n""")
+    makefile_path_a.write_text("""task(name="a",requires=["Makexfile-b:b"])\n""")
 
     makefile_path_b = tmp_path / "Makexfile-b"
-    makefile_path_b.write_text("""target(name="b",requires=["Makexfile-a:a"])\n""")
+    makefile_path_b.write_text("""task(name="b",requires=["Makexfile-a:a"])\n""")
 
     ctx = Context()
     ctx.workspace_object = Workspace(tmp_path)
     graph = TargetGraph()
 
     result = parse_makefile_into_graph(ctx, makefile_path_a, graph, allow_makex_files=True)
 
@@ -71,17 +72,15 @@
 
 
 def test_cycle_error_internal_targets(tmp_path: Path):
     """
     Test cycles between targets inside the same file.
     """
     makefile_path = tmp_path / "Makexfile"
-    makefile_path.write_text(
-        """target(name="a",requires=[":b"])\ntarget(name="b",requires=[":a"])\n"""
-    )
+    makefile_path.write_text("""task(name="a",requires=[":b"])\ntask(name="b",requires=[":a"])\n""")
 
     ctx = Context()
     ctx.workspace_object = Workspace(tmp_path)
     graph = TargetGraph()
 
     result = parse_makefile_into_graph(ctx, makefile_path, graph)
 
@@ -112,22 +111,21 @@
     workspace_b = tmp_path / "nested"
     workspace_b.mkdir(parents=True)
 
     workspace_file_a = workspace_a / "WORKSPACE"
     workspace_file_a.touch()
 
     makefile_path_a = workspace_a / "Makexfile"
-    makefile_path_a.write_text("""target("a", requires=[])""")
+    makefile_path_a.write_text("""task("a", requires=[])""")
 
     workspace_file_b = workspace_b / "WORKSPACE"
     workspace_file_b.touch()
 
     makefile_path_b = workspace_b / "Makexfile"
-    makefile_path_b.write_text("""target("b", requires=["//..:b"])""")
-
+    makefile_path_b.write_text("""task("b", requires=["//..:b"])""")
 
     ctx = Context()
     ctx.workspace_object = Workspace(tmp_path)
     graph = TargetGraph()
 
     result = parse_makefile_into_graph(ctx, makefile_path_b, graph)
 
@@ -139,31 +137,110 @@
     workspace_b = tmp_path / "nested"
     workspace_b.mkdir(parents=True)
 
     workspace_file_a = workspace_a / "WORKSPACE"
     workspace_file_a.touch()
 
     makefile_path_a = workspace_a / "Makexfile"
-    makefile_path_a.write_text("""target("a", requires=["//nested:b"])""")
+    makefile_path_a.write_text("""task(name="a", requires=["//nested:b"])""")
 
     workspace_file_b = workspace_b / "WORKSPACE"
     workspace_file_b.touch()
 
     makefile_path_b = workspace_b / "Makexfile"
-    makefile_path_b.write_text("""target("b", requires=[])""")
+    makefile_path_b.write_text("""task(name="b", requires=[])""")
 
     ctx = Context()
     ctx.workspace_object = Workspace(tmp_path)
     graph = TargetGraph()
 
     result = parse_makefile_into_graph(ctx, makefile_path_a, graph)
     ref_a = ResolvedTargetReference("a", makefile_path_a)
 
     a = graph.get_target(ref_a)
 
+    assert not result.errors
+
     assert a
     assert a.requires
     assert len(a.requires)
-    assert not result.errors
+
     #assert a.requires == [ResolvedTargetReference("b", "//nested")]
 
 
+def test_include_macros(tmp_path: Path):
+    workspace_a = tmp_path
+    workspace_file_a = workspace_a / "WORKSPACE"
+    workspace_file_a.touch()
+
+    makefile_path_a = workspace_a / "Makexfile"
+    makefile_path_a.write_text("""include("include.mx"); test()""")
+
+    makefile_path_b = workspace_a / "include.mx"
+    makefile_path_b.write_text("""@macro
+def test():
+  task(name="test")
+""")
+
+    ctx = Context()
+    ctx.workspace_object = Workspace(tmp_path)
+    graph = TargetGraph()
+
+    result = parse_makefile_into_graph(ctx, makefile_path_a, graph)
+    ref_a = ResolvedTargetReference("test", makefile_path_a)
+
+    a = graph.get_target(ref_a)
+    assert a
+
+
+def test_include_targets(tmp_path: Path):
+    workspace_a = tmp_path
+    workspace_file_a = workspace_a / "WORKSPACE"
+    workspace_file_a.touch()
+
+    makefile_path_a = workspace_a / "Makexfile"
+    makefile_path_a.write_text("""include("include.mx", tasks=True); task(name="a")""")
+
+    makefile_path_b = workspace_a / "include.mx"
+    makefile_path_b.write_text("""task(name="b")""")
+
+    ctx = Context()
+    ctx.workspace_object = Workspace(tmp_path)
+    graph = TargetGraph()
+
+    result = parse_makefile_into_graph(ctx, makefile_path_a, graph)
+    ref_a = ResolvedTargetReference("b", makefile_path_a)
+
+    a = graph.get_target(ref_a)
+    assert a
+
+    ref_a = ResolvedTargetReference("a", makefile_path_a)
+    a = graph.get_target(ref_a)
+
+    assert a
+
+
+@pytest.mark.skip
+def test_import_macros(tmp_path: Path):
+    # TODO: enable flag or weave a variable into ctx so that this can work
+    workspace_a = tmp_path
+    workspace_file_a = workspace_a / "WORKSPACE"
+    workspace_file_a.touch()
+
+    makefile_path_a = workspace_a / "Makexfile"
+    makefile_path_a.write_text("""from include import test; test()""")
+
+    makefile_path_b = workspace_a / "include.mx"
+    makefile_path_b.write_text("""@macro
+def test():
+  task(name="test")
+""")
+
+    ctx = Context()
+    ctx.workspace_object = Workspace(tmp_path)
+    graph = TargetGraph()
+
+    result = parse_makefile_into_graph(ctx, makefile_path_a, graph)
+    ref_a = ResolvedTargetReference("test", makefile_path_a)
+
+    a = graph.get_target(ref_a)
+    assert a
```

### Comparing `makex-20240203/python/makex/metadata.py` & `makex-20240401/python/makex/metadata.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
-from datetime import datetime, timezone
-from typing import Protocol, Optional
+from datetime import (
+    datetime,
+    timezone,
+)
+from typing import (
+    Optional,
+    Protocol,
+)
 
 from makex.context import Context
 from makex.protocols import StringHashFunction
 from makex.python_script import FileLocation
 from makex.target import EvaluatedTarget
 
 
@@ -78,16 +84,17 @@
 
 
 #class FileLocation:
 #    line:int
 #    column:int
 #    path:str
 
+
 class TargetMetadata:
-    # TODO: we should be able to serialize runnables/arguments
+    # TODO: we should be able to serialize Actions/arguments
     name: str
     path: str
     key: str
 
     # where this target came from
     location: FileLocation
 
@@ -127,15 +134,21 @@
 
         for requirement in d.get("requires"):
             r = Requirement.from_json(requirement)
             requires[r.hash] = r
         return c
 
     @classmethod
-    def from_evaluated_target(cls, ctx:Context, target:EvaluatedTarget, hash_function:StringHashFunction, timing=None) -> "TargetMetadata":
+    def from_evaluated_target(
+        cls,
+        ctx: Context,
+        target: EvaluatedTarget,
+        hash_function: StringHashFunction,
+        timing=None
+    ) -> "TargetMetadata":
         c = cls()
         c.name = target.name
         c.path = target.path.as_posix()
         c.key = target.key()
 
         c.hash = target.hash(ctx, hash_function=hash_function)
 
@@ -146,15 +159,15 @@
         c.location = target.location
         c.time = datetime.now(timezone.utc)
 
         if timing:
             c.start_time, c.end_time = timing
         for requirement in target.requires or []:
             requirement.key()
-            requirement.hash(ctx, hash_function=hash())
+            requirement.hash(ctx, hash_function=hash_function)
         return c
 
     def dirty(self, ctx: Context, target: EvaluatedTarget) -> Dirtyness:
         # TODO: we don' really need this at the moment.
         # Manually evaluate the dirtyness of a target.
 
         # TargetMetadata.hash == target.hash()
@@ -197,13 +210,12 @@
         return Dirtyness()
 
 
 class MetadataProtocol(Protocol):
     """
     Metadata [backend] protocol. This should be fast and synchronous.
     """
-    def get_target(self, target_hash:str)-> Optional[TargetMetadata]:
+    def get_target(self, target_hash: str) -> Optional[TargetMetadata]:
         pass
 
-    def put_target(self, target:TargetMetadata) -> Optional[Exception]:
+    def put_target(self, target: TargetMetadata) -> Optional[Exception]:
         pass
-
```

### Comparing `makex-20240203/python/makex/metadata_file.py` & `makex-20240401/python/makex/metadata_file.py`

 * *Files identical despite different names*

### Comparing `makex-20240203/python/makex/metadata_sqlite.py` & `makex-20240401/python/makex/metadata_sqlite.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 from datetime import (
     datetime,
     timezone,
 )
 from pathlib import Path
 from typing import Optional
 
-from makex._logging import debug
+from makex._logging import debug, info
 from makex.file_checksum import FileChecksum
 
-DATABASE_VERSION = 2
+DATABASE_VERSION = 3
 
 
 @contextmanager
 def transaction(conn):
     # From: https://charlesleifer.com/blog/going-fast-with-sqlite-and-python/
     # We must issue a "BEGIN" explicitly when running in auto-commit mode.
     conn.execute('BEGIN')
@@ -24,14 +24,21 @@
     except Exception as e:
         conn.rollback() # Roll back all changes if an exception occurs.
         raise e
     else:
         conn.commit()
 
 
+def upgrade_3(backend: "SqliteMetadataBackend"):
+    result = backend._execute("DROP TABLE IF EXISTS files")
+    result = backend._execute(
+        "CREATE TABLE IF NOT EXISTS files (path TEXT, fingerprint TEXT, checksum_type TEXT, checksum TEXT,  date TEXT)"
+    )
+    backend._execute(f"PRAGMA user_version=3")
+
 class SqliteMetadataBackend:
     def __init__(self, path: Path):
         debug("Connecting to sqlite database at %s", path)
         self.con = sqlite3.connect(path.as_posix())
         self.cur = self.con.cursor()
         # raise a database needs upgrade error.
         self.cur.execute("PRAGMA journal_mode=WAL")
@@ -39,22 +46,26 @@
         self.cur.execute("PRAGMA cache_size=-16000")
         # mmap size is zero by default (disabled). increase it to 20MB.
         # https://sqlite.org/mmap.html
         self.cur.execute("PRAGMA mmap_size=20000000")
 
         # TODO: check user_version pragma to check if our schema is still valid
         version = self._get_one("PRAGMA user_version")
-        if version is not None:
-            debug("DB Version %s", version)
+
+        debug("Database version %s < %s", version, DATABASE_VERSION)
+
+        if version is not None and version > 0:
             version = int(version)
 
-            if version < DATABASE_VERSION:
-                debug("Upgrading database...")
+            if version == 2:
+                info("Upgrading database to version 3...")
                 # move any old database file before initialization
-                self.initialize()
+                #if version == 2:
+                upgrade_3(self)
+                version = 3
         else:
             self.initialize()
 
         # TODO: use an LRU here to keep hot things
         self._target_cache = {}
 
     def _execute(self, query, *args):
@@ -72,17 +83,19 @@
         res = self.cur.execute(query, args)
         result = res.fetchone()
         if result is None:
             return None
 
         return result
 
-    def has_target(self, target_hash: str) -> bool:
+    def has_target(self, target_key: str, target_hash: str) -> bool:
         # return true if the db has the target with a hash (it was executed).
-        count = self._get_one("SELECT count(*) FROM targets WHERE hash = ?", target_hash)
+        count = self._get_one(
+            "SELECT count(*) FROM targets WHERE key = ? AND hash = ?", target_key, target_hash
+        )
         if count:
             return True
 
         return False
 
     def put_target(self, key, target_hash):
         time = datetime.now(timezone.utc)
@@ -95,32 +108,39 @@
             "SELECT count(*) FROM files WHERE path = ? AND fingerprint = ?", path, fingerprint
         )
         if count:
             return True
 
         return False
 
-    def get_file_checksum(self, path:str, fingerprint:str) -> Optional[FileChecksum]:
+    def get_file_checksum(self, path: str, fingerprint: str) -> Optional[FileChecksum]:
         count = self._get_row(
-            "SELECT checksum_type, checksum FROM files WHERE path = ? AND fingerprint = ?", path, fingerprint
+            "SELECT checksum_type, checksum FROM files WHERE path = ? AND fingerprint = ?",
+            path,
+            fingerprint
         )
         if count is None:
             return None
 
         return FileChecksum(FileChecksum.Type(count[0]), count[1], fingerprint)
 
-    def put_file(self, path:str, fingerprint:str, checksum_type:str, checksum:str):
+    def put_file(self, path: str, fingerprint: str, checksum_type: str, checksum: str):
         # store checksums for input/output files (out of band)
         # tombstone/delete any other records for file
         time = datetime.now(timezone.utc)
         time = time.strftime("%Y-%m-%d %H:%M:%S")
         try:
             with transaction(self.con):
                 self._execute(
-                    "INSERT into files values (?, ?, ?, ?, ?)", path, fingerprint, checksum_type, checksum, time
+                    "INSERT into files values (?, ?, ?, ?, ?)",
+                    path,
+                    fingerprint,
+                    checksum_type,
+                    checksum,
+                    time
                 )
         except sqlite3.IntegrityError as e:
             raise e
 
     def initialize(self):
         cur = self.cur
         with transaction(self.con):
@@ -135,10 +155,9 @@
                 "CREATE TABLE IF NOT EXISTS files (path TEXT, fingerprint TEXT, checksum_type TEXT, checksum TEXT,  date TEXT)"
             )
             self._execute(f"PRAGMA user_version={DATABASE_VERSION}")
 
     def clear(self):
 
         with self.con:
-            res = self.con.execute("delete from targets")
-            res = self.con.execute("delete from files")
-
+            res = self._execute("delete from targets")
+            res = self._execute("delete from files")
```

### Comparing `makex-20240203/python/makex/patterns.py` & `makex-20240401/python/makex/patterns.py`

 * *Files identical despite different names*

### Comparing `makex-20240203/python/makex/patterns_test.py` & `makex-20240401/python/makex/patterns_test.py`

 * *Files identical despite different names*

### Comparing `makex-20240203/python/makex/platform_object/platform_object.py` & `makex-20240401/python/makex/platform_object/platform_object.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import logging
 import operator
 from enum import Enum
+from logging import debug
 from typing import (
     Any,
+    Callable,
     Hashable,
     Union,
 )
 
-from logging import debug
-
 
 class PlatformTestObject:
     def __init__(self):
         pass
 
 
 PlatformRight = Any
@@ -35,74 +34,84 @@
     return not operator.contains(a, b)
 
 
 def one_of(a, b):
     return operator.contains(b, a)
 
 
-op_map = {
+op_map: dict[Operator, Callable[[Any, Any], bool]] = {
     Operator.IN: one_of,
     Operator.LTE: operator.le,
     Operator.GT: operator.gt,
     Operator.NOT_IN: not_in,
     Operator.EQ: operator.eq,
     Operator.NE: operator.ne,
     Operator.LT: operator.lt,
     Operator.GTE: operator.ge,
     Operator.AND: operator.and_,
     Operator.OR: operator.or_,
 }
 
 
 class PlatformCondition:
-    left: "PlatformLeft"
+    left: Union["PlatformCondition", "PlatformLeft"]
     operator: Operator
     right: PlatformRight
 
     def __init__(
         self,
-        left: Union["PlatformLeft", "PlatformCondition"],
+        left: Union["PlatformCondition", "PlatformLeft"],
         operator: Operator,
         right: PlatformRight
     ):
         self.left = left
         self.operator = operator
         self.right = right
 
     def __repr__(self):
-        #def __str__(self):
         inside = " ".join((repr(self.left), str(self.operator), str(self.right)))
         return f"({inside})"
 
     def __hash__(self):
         return hash(self.left)
 
-    def __eq__(self, other: "PlatformLeft"):
-        d = {other.name: other.value}
+    def __eq__(self, other: Any):
+        name = getattr(other, "name", None)
+        if name is None:
+            return False
+
+        value = getattr(other, "value", None)
+
+        if value is None:
+            return False
+
+        d = {name: value}
         r = self.evaluate(d)
         debug("Evaluated %s: %s = %s", self, d, r)
-
         return r
 
     def returns(self, value):
-
         pass
 
-    def evaluate(self, platform: dict[Hashable, Any]):
+    def evaluate(self, platform: dict[Hashable, Any]) -> bool:
         if self.operator == Operator.AND:
-            left_value = self.left.evaluate(platform)
+            left_value = self.left.evaluate(platform) if isinstance(
+                self.left, PlatformCondition
+            ) else self.left.value
             right_value = self.right.evaluate(platform)
             return bool(left_value and right_value)
         elif self.operator == Operator.OR:
-            left_value = self.left.evaluate(platform)
+            left_value = self.left.evaluate(platform) if isinstance(
+                self.left, PlatformCondition
+            ) else self.left.value
             right_value = self.right.evaluate(platform)
             return bool(left_value or right_value)
 
         left_value = platform.get(self.left)
-        op = op_map.get(self.operator)
+        op = op_map[self.operator]
         return op(left_value, self.right)
 
     def __and__(self, other) -> "PlatformCondition":
         """
         c & b & d
 
         ((c, and, b), and, d)
@@ -189,11 +198,7 @@
     #location:FileLocation
 
     def __init__(self, values):
         self.values = values
         self.os_type = PlatformLeft("os_type", values.get("os_type", None))
         self.architecture = PlatformLeft("architecture", values.get("architecture", None))
 
-    #    self.location = None
-
-    #def with_location(self, location:FileLocation) -> PlatformObject:
-    #    self.location = location
```

### Comparing `makex-20240203/python/makex/protocols.py` & `makex-20240401/python/makex/protocols.py`

 * *Files identical despite different names*

### Comparing `makex-20240203/python/makex/python_script.py` & `makex-20240401/python/makex/python_script.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,34 +7,40 @@
 - Do not split items in this file into separate modules/packages.
 
 """
 import ast
 import logging
 import sys
 import traceback
+import types
 from abc import (
     ABC,
     abstractmethod,
 )
 from collections import deque
 from copy import copy
+from importlib.machinery import ModuleSpec
 from io import StringIO
 from os import PathLike
 from pathlib import Path
 from typing import (
     Any,
     BinaryIO,
+    Optional,
     Protocol,
+    Union,
 )
 
 LOGGER = logging.getLogger("python-script")
 STRING_VALUE_NAME = "_STRING_"
 LIST_VALUE_NAME = "_LIST_"
+GLOBALS_NAME = "_GLOBALS_"
 FILE_LOCATION_NAME = "_LOCATION_"
 FILE_LOCATION_ARGUMENT_NAME = "_location_"
+FILE_LOCATION_ATTRIBUTE = "location"
 
 
 class FileLocation:
     line: int
     column: int
     path: str
 
@@ -48,23 +54,79 @@
 
     def __repr__(self):
         if self.path:
             return f"FileLocation({self.line}, {self.column}, \"{self.path}\")"
         else:
             return f"FileLocation({self.line}, {self.column})"
 
+    def __str__(self):
+        if self.path:
+            return f"{self.path}:{self.line}:{self.column}"
+        else:
+            return f"{self.line}:{self.column}"
+
+    @classmethod
+    def from_ast_node(self, node: ast, path: str):
+        return FileLocation(
+            line=node.lineno,
+            column=node.col_offset,
+            path=path,
+        )
+
+
+_SENTINEL = object()
+
+
+def get_location(object, default=_SENTINEL) -> Optional[FileLocation]:
+    # Return a FileLocation from an object in a python script.
+    if default is _SENTINEL:
+        return getattr(object, FILE_LOCATION_ATTRIBUTE)
+    return getattr(object, FILE_LOCATION_ATTRIBUTE, default)
+
+
+def is_function_call(node: ast.Call, name: str):
+    if isinstance(node, ast.Call) is False:
+        return False
+
+    if isinstance(node.func, ast.Name) and node.func.id == name:
+        return True
+
+    return False
+
+
+def call_function(name, line, column, args=None, keywords=None):
+    call = ast.Call(
+        func=ast.Name(
+            id=name,
+            ctx=ast.Load(),
+            lineno=line,
+            col_offset=column,
+        ),
+        args=args or [],
+        keywords=keywords or [],
+        lineno=line,
+        col_offset=column,
+    )
+    return call
+
 
 class ScriptCallable:
     def __call__(self, *args, _line_: int, _column_: int, **kwargs):
         pass
 
 
 class ScriptEnvironment(Protocol):
+    # TODO: abc this. We should call and use globals() in descendant environments so StringValue/etc work.
     def globals(self) -> dict[str, ScriptCallable]:
-        pass
+        return {
+            STRING_VALUE_NAME: StringValue,
+            LIST_VALUE_NAME: ListValue,
+            GLOBALS_NAME: globals,
+            FILE_LOCATION_NAME: FileLocation
+        }
 
 
 Globals = dict[str, str]
 
 
 class BaseScriptEnvironment(ABC):
     def exit(self):
@@ -160,37 +222,37 @@
 
     # TODO: __add__ with a non-string should return an internal JoinedString
 
 
 class DisableImports(ast.NodeVisitor):
     # TODO: disable imports
 
-    def __init__(self, path: Path):
-        self.path = path.as_posix()
+    def __init__(self, path: PathLike):
+        self.path = path
 
     def visit_Import(self, node):
         print(
             f"""Line {node.lineno} imports modules {
         ', '.join(alias.name for alias in node.names)
         }"""
         )
         raise PythonScriptError(
             "Invalid syntax (Imports are not allowed):",
-            FileLocation(node.lineno, node.col_offset, self.path)
+            FileLocation.from_ast_node(node, self.path)
         )
 
     def visit_ImportFrom(self, node):
         print(
             f"""Line {node.lineno} imports from module {node.module} the names {
         ', '.join(alias.name for alias in node.names)
         }"""
         )
         raise PythonScriptError(
             "Invalid syntax (Imports are not allowed):",
-            FileLocation(node.lineno, node.col_offset, self.path)
+            FileLocation.from_ast_node(node, self.path)
         )
 
 
 def _create_file_location_call(path, line, column):
     file_location_call = ast.Call(
         func=ast.Name(
             id=FILE_LOCATION_NAME,
@@ -206,14 +268,69 @@
         keywords=[],
         lineno=line,
         col_offset=column,
     )
     return file_location_call
 
 
+class _DisableAssignments(ast.NodeVisitor):
+    """
+    Disable assignments:
+    - to anything non-script (globals)
+    - to specified variables.
+
+    a,b = item
+    a,*b = it
+
+    del a
+
+    a = 1
+    """
+    def __init__(self, path: PathLike, names: set = None):
+        self.path = str(path)
+        self.names = names or set()
+
+    def check_name(self, node, name):
+        if name in self.names:
+            raise PythonScriptError(
+                f"Can't assign to the name '{name}'. Please rename the variable to something else.",
+                location=FileLocation.from_ast_node(node, self.path),
+            )
+
+    def visit_NamedExpr(self, node: ast.NamedExpr) -> Any:
+        # (walrus)
+        if isinstance(node.target, ast.Name):
+            self.check_name(node, node.target.id)
+
+    def visit_AnnAssign(self, node: ast.AnnAssign) -> Any:
+        #AnnAssign; assignments with type expressions
+        if isinstance(node.target, ast.Name):
+            self.check_name(node, node.target.id)
+
+    def visit_Assign(self, node: ast.Assign) -> Any:
+        for target in node.targets:
+            if isinstance(target, ast.Name):
+                self.check_name(node, target.id)
+            elif isinstance(target, ast.Tuple):
+                for element in target.elts:
+                    if isinstance(element, ast.Name):
+                        self.check_name(element, element.id)
+        """
+         the following expression can appear in assignment context
+
+         | Attribute(expr value, identifier attr, expr_context ctx)
+         | Subscript(expr value, expr slice, expr_context ctx)
+         | Starred(expr value, expr_context ctx)
+         | Name(identifier id, expr_context ctx)
+         | List(expr* elts, expr_context ctx)
+         | Tuple(expr* elts, expr_context ctx)
+
+        """
+
+
 class _TransformStringValues(ast.NodeTransformer):
     """
     Transform string and f-strings to be wrapped in a StringValue() with a FileLocation.
     """
     def __init__(self, path: PathLike):
         self.path = path
 
@@ -223,73 +340,82 @@
             # return the node and don't process the FileLocation children.
             return node
         self.generic_visit(node)
         return node
 
     def visit_Constant(self, node: ast.Constant) -> Any:
         if isinstance(node.value, str):
+            line = node.lineno
+            offset = node.col_offset
+
             #logging.debug("Got string cnst %s %s", node.value, node.lineno)
-            file_location = _create_file_location_call(self.path, node.lineno, node.col_offset)
+            file_location = _create_file_location_call(self.path, line, offset)
 
             # TODO: separate the values into JoinedString class so we can evaluate later.
             strcall = ast.Call(
                 func=ast.Name(
                     id=STRING_VALUE_NAME,
                     ctx=ast.Load(),
-                    lineno=node.lineno,
-                    col_offset=node.col_offset,
+                    lineno=line,
+                    col_offset=offset,
                 ),
                 args=[node],
                 keywords=[
                     ast.keyword(
                         arg='location',
                         value=file_location,
-                        lineno=node.lineno,
-                        col_offset=node.col_offset,
+                        lineno=line,
+                        col_offset=offset,
                     ),
                 ],
-                lineno=node.lineno,
-                col_offset=node.col_offset,
+                lineno=line,
+                col_offset=offset,
             )
             return strcall
         else:
             #logging.debug("Got other const %r", node.value)
             return node
 
     def visit_JoinedStr(self, node: ast.JoinedStr) -> Any:
-        file_location = _create_file_location_call(self.path, node.lineno, node.col_offset)
+        line = node.lineno
+        offset = node.col_offset
+
+        file_location = _create_file_location_call(self.path, line, offset)
 
         # TODO: separate the values into JoinedString class so we can evaluate later.
         strcall = ast.Call(
             func=ast.Name(id=STRING_VALUE_NAME, ctx=ast.Load()),
             args=[node],
             keywords=[
                 ast.keyword(arg='location', value=file_location),
             ],
-            lineno=node.lineno,
-            col_offset=node.col_offset,
+            lineno=line,
+            col_offset=offset,
         )
         self.generic_visit(node)
 
         ast.fix_missing_locations(strcall)
         return strcall
 
     # XXX: Deprecated in 3.8 and unused past that version.
     def visit_Str(self, node):
         self.generic_visit(node)
 
-        file_location = _create_file_location_call(self.path, node.lineno, node.col_offset)
+        line = node.lineno
+        offset = node.col_offset
+
+        file_location = _create_file_location_call(self.path, line, offset)
         strcall = ast.Call(
             func=ast.Name(id=STRING_VALUE_NAME, ctx=ast.Load()),
             args=[ast.Str(node.s)],
             keywords=[
                 ast.keyword(arg='location', value=file_location),
             ],
-            lineno=node.lineno,
-            col_offset=node.col_offset,
+            lineno=line,
+            col_offset=offset,
         )
 
         ast.fix_missing_locations(strcall)
         return strcall
 
 
 class _TransformCallsToHaveFileLocation(ast.NodeTransformer):
@@ -430,89 +556,189 @@
     def __init__(self, path: str):
         self.path = path
 
     def visit_List(self, node):
         #if len(node.elts) > 0:
         #    return ast.copy_location(node, node)
         #return ast.copy_location(ast.NameConstant(value=None), node)
+        line = node.lineno
+        offset = node.col_offset
+
         _node = ast.Call(
-            func=ast.Name(
-                id=LIST_VALUE_NAME, ctx=ast.Load(), lineno=node.lineno, col_offset=node.col_offset
-            ),
+            func=ast.Name(id=LIST_VALUE_NAME, ctx=ast.Load(), lineno=line, col_offset=offset),
             args=[node],
             keywords=[],
-            lineno=node.lineno,
-            col_offset=node.col_offset,
+            lineno=line,
+            col_offset=offset,
         )
 
-        file_location = _create_file_location_call(self.path, node.lineno, node.col_offset)
+        file_location = _create_file_location_call(self.path, line, offset)
         _node.keywords.append(
             ast.keyword(
                 arg=FILE_LOCATION_ARGUMENT_NAME,
                 value=file_location,
-                lineno=node.lineno,
-                col_offset=node.col_offset
+                lineno=line,
+                col_offset=offset
             )
         )
 
         #for child in ast.iter_child_nodes(node):
         #    self.visit(child)
 
         #ast.fix_missing_locations(_node)
         self.generic_visit(node)
         return _node
 
     visit_ListComp = visit_List
 
 
 class PythonScriptFile:
-    def __init__(self, path: PathLike, env: ScriptEnvironment, globals: Globals = None):
-        self._env = env
+    def __init__(
+        self,
+        path: PathLike,
+        globals: Globals = None,
+        importer=None,
+        pre_visitors=None,
+        extra_visitors=None,
+        enable_imports=False,
+    ):
+        #self._env = env
         self.path = str(path)
         self.globals = globals or {}
+        self.disable_assignment_names = set()
+        self.extra_visitors = extra_visitors or []
+        self.pre_visitors = pre_visitors or []
+        self.enable_imports = enable_imports
+        self.importer = importer or self._importer
+
         # transform attribute calls to have line/column information
+        #self._all_globals = self._env.globals()
+        #self._all_globals.update(self.globals)
 
     def _ast_parse(self, f: BinaryIO):
         # XXX: must be binary due to the way hash_contents works
         buildfile_contents = f.read()
         f.seek(0)
         # transform to ast
         tree = ast.parse(buildfile_contents, filename=self.path, mode='exec')
         return tree
 
-    def execute(self, file: BinaryIO):
+    def set_disabled_assignment_names(self, names: set):
+        self.disable_assignment_names = names
+
+    #def _get_env_attr(self, name):
+    #    if self._env.has_global(name):
+    #        return self._env.get_global(name)
+
+    #    try:
+    #        return self._all_globals.get(name)
+    #    except ValueError as e:
+    #        raise PythonScriptError(f"{name} not defined in global scope.")
+
+    def parse(self, file: Union[BinaryIO]) -> ast.AST:
+        # parse and process the ast.
+        # TODO: prefix the modules to execute with the ast to include
         try:
             tree = self._ast_parse(file)
         except SyntaxError as e:
             exc_type, exc_message, exc_traceback = sys.exc_info()
             l = FileLocation(e.lineno, e.offset, self.path)
             raise PythonScriptError(e, location=l) from e
 
-        scope = self._env.globals()
-        scope.update(self.globals)
+        self._parse(tree)
+
+        return tree
 
+    def _parse(self, tree: ast.AST):
         # set of names to ignore
-        ignore = {STRING_VALUE_NAME, FILE_LOCATION_NAME, LIST_VALUE_NAME}
+        ignore = {STRING_VALUE_NAME, FILE_LOCATION_NAME, LIST_VALUE_NAME, GLOBALS_NAME}
+
+        # Catch some early errors
+        if False:
+            t = DisableImports(self.path)
+            t.visit(tree)
+
+        t = _DisableAssignments(self.path, self.disable_assignment_names)
+        t.visit(tree)
+
+        for visitor in self.pre_visitors:
+            visitor.visit(tree)
 
         # XXX: calls should be transformed first
         t = _TransformCallsToHaveFileLocation(ignore, self.path)
         t.visit(tree)
 
         # XXX: string values and primitives should be transformed next
         t = _TransformStringValues(self.path)
         t.visit(tree)
 
         t = _TransformListValues(self.path)
         t.visit(tree)
 
+        for visitor in self.extra_visitors:
+            visitor.visit(tree)
+
+    def _importer(self, name, globals=None, locals=None, fromlist=(), level=0):
+        # level = 1 if relative import. e.g from .module import item
+        # TODO: improve this error location
+        raise ImportError("Imports are disabled here.")
+
+    def execute(self, tree: ast.AST):
+        if not isinstance(tree, ast.AST):
+            raise ValueError(f"Expected AST argument. Got {type(tree)}")
+            # TODO: use hasattr(file, "read") instead of isinstance
+            #tree = file
+        #else:
+        #    tree = self.parse(file)
+        from importlib.abc import Loader
+
+        class CustomModule(types.ModuleType):
+            def __init__(self, name):
+                super().__init__(name)
+                self.macros = {}
+
+            def __getattribute__(self, item):
+                if item == "__dict__":
+                    return self.__dict__
+
+                macro = self.macros.get(item, None)
+
+                if macro is None:
+                    raise PythonScriptError(
+                        f"Can't import {item} from {self.name}", FileLocation(0, 0, "//")
+                    )
+                return macro
+
+        class MakexLoader(Loader):
+            def create_module(self, spec: ModuleSpec) -> Union[types.ModuleType, None]:
+                print("CREATING MODULE", spec)
+                module = types.ModuleType(spec.name)
+                #exec(code, module.__dict__)
+
+                return module
+
+            def exec_module(self, module: types.ModuleType) -> None:
+                print("Exec module", module)
+                pass
+
+        #scope = self._env.globals()
+        #scope.update(self.globals)
+        scope = self.globals
+        #scope["__getattr__"] = self._get_env_attr
+
+        scope["__builtins__"] = {}
+
+        if self.enable_imports:
+            scope["__builtins__"] = {"__import__": self.importer}
         #print(ast.dump(tree, indent=2))
 
         scope[STRING_VALUE_NAME] = StringValue
         scope[FILE_LOCATION_NAME] = FileLocation
         scope[LIST_VALUE_NAME] = ListValue
+        scope[GLOBALS_NAME] = globals
 
         try:
             code = compile(tree, self.path, 'exec')
             exec(code, scope, scope)
         except TypeError as e:
             #LOGGER.exception(e)
             exc_type, exc_message, exc_traceback = sys.exc_info()
@@ -524,37 +750,51 @@
                     location = FileLocation(item.lineno, 0, self.path)
                     break
             else:
                 last = tb1.stack[-1]
                 location = FileLocation(last.lineno, 0, self.path)
             raise PythonScriptError(e, location=location) from e
 
-        except (IndexError, NameError) as e:
+        except (IndexError, NameError, AttributeError) as e:
             #LOGGER.exception(e)
             exc_type, exc_message, exc_traceback = sys.exc_info()
             # COMPAT: PYTHON 3.5+
             tb1 = traceback.TracebackException.from_exception(e)
             last = tb1.stack[-1]
-            l = FileLocation(last.lineno, 0, self.path)
+
+            l = FileLocation(last.lineno, 0, last.filename)
+            for item in tb1.stack:
+                print("TRACE", item)
+                #if item.filename == self.path:
+                #    location = FileLocation(item.lineno, 0, self.path)
+                #    break
+
             raise PythonScriptError(e, location=l) from e
 
         except StopPythonScript as e:
             # python script exited
             #LOGGER.exception(e)
             tb1 = traceback.TracebackException.from_exception(e)
             last = tb1.stack[-1]
             l = FileLocation(last.lineno, 0, self.path)
             raise PythonScriptError(e, location=l) from e
 
+        except ImportError as e:
+            tb1 = traceback.TracebackException.from_exception(e)
+            last = tb1.stack[-1]
+            l = FileLocation(last.lineno, 0, self.path)
+            raise PythonScriptError(e, location=l) from e
         except SyntaxError as e:
             #LOGGER.exception(e)
             exc_type, exc_message, exc_traceback = sys.exc_info()
             l = FileLocation(e.lineno, e.offset, self.path)
             raise PythonScriptError(e, location=l) from e
 
+        return code
+
 
 def pretty_exception(exception, location: FileLocation):
     # TODO: remove colors from this pretty_exception
     buf = StringIO()
     buf.write(f"Error inside a Makexfile '{location.path}:{location.line}'\n\n")
     buf.write(f"{exception}\n\n")
     with Path(location.path).open("r") as f:
```

### Comparing `makex-20240203/python/makex/run.py` & `makex-20240401/python/makex/run.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,29 @@
 from collections import deque
 from io import StringIO
 from pathlib import Path
 from threading import local
 
 from makex.protocols import CommandOutput
 
+CORRECTED_RETURN_CODE = object()
+
 _QUEUE = deque()
 
 
 def get_running_process_ids():
     return _QUEUE
 
 
 def is_exe(path):
     return path.is_file() and os.access(path, os.X_OK)
 
 
 def check_exec(path):
-    if not is_exe(path):
+    if is_exe(path) is False:
         raise Exception(f"Command is not executable: {path}. Fix this with chmod +x {path}")
 
 
 _thread_local = local()
 
 
 def _kill_sub():
@@ -103,23 +105,24 @@
             outputs = outputs.getvalue()
             errors = errors.getvalue()
         else:
             outputs = None
             errors = None
             tail_out(sel, p)
 
-        returnCode = p.poll()
+        return_code = p.wait()
 
         _thread_local.process = None
 
         _QUEUE.remove(p.pid)
         # XXX: For some reason this was returning None when everything was actually ok. (on linux,el8)
-        if returnCode is None:
-            returnCode = 0
-        return CommandOutput(returnCode, outputs, errors)
+        if return_code is None:
+            return_code = CORRECTED_RETURN_CODE
+
+        return CommandOutput(return_code, outputs, errors)
 
 
 def tail_out(sel, p, enable_output=True, color_error="", color_escape=""):
     while True:
         for key, _ in sel.select():
             data = key.fileobj.read1().decode()
             if not data:
@@ -129,15 +132,14 @@
                     print(
                         data,
                         end="",
                         flush=True,
                     )
                 yield data, None
             else:
-                #print(data, end="", file=sys.stderr)
                 if enable_output:
                     print(
                         f"{color_error}ERROR OUTPUT:{color_escape} {data}",
                         end="",
                         file=sys.stderr,
                         flush=True,
                     )
```

### Comparing `makex-20240203/python/makex/target.py` & `makex-20240401/python/makex/target.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,158 +7,171 @@
 from pathlib import Path
 from typing import (
     Any,
     Iterable,
     Optional,
     Protocol,
     Type,
+    Union,
 )
 
 from makex._logging import (
     debug,
     trace,
 )
+from makex.constants import HASHING_ALGORITHM
 from makex.context import Context
 from makex.protocols import (
     CommandOutput,
     FileStatus,
     StringHashFunction,
 )
 from makex.python_script import FileLocation
 from makex.workspace import Workspace
 
 TargetKey = str
 
+HASH_FUNCTION = getattr(hashlib, HASHING_ALGORITHM, "sha1")
+
 
 class TargetBase(ABC):
     name: str
 
     @abstractmethod
     def key(self) -> TargetKey:
         raise NotImplementedError()
         #return format_hash_key(self.name, self.path)
 
 
-class Runnable(Protocol):
+class Action(Protocol):
     location: FileLocation
 
     def __call__(self, ctx: Context, target: "EvaluatedTarget") -> CommandOutput:
-        # old runnable function
+        # old Action function
         ...
 
     def run_with_arguments(
         self, ctx: Context, target: "EvaluatedTarget", arguments: dict[str, Any]
     ) -> CommandOutput:
         ...
 
     def hash(self, ctx: Context, arguments: dict[str, Any], hash_function: StringHashFunction):
-        # allow runnables to produce a hash of their arguments
+        # allow Actions to produce a hash of their arguments
         # if anything about them changes (e.g. arguments/inputs/checksums) the hash should change
         return
 
 
-class InternalRunnable:
+class InternalAction:
     """
-    Keep an Internal runnable that records the arguments evaluated from a runnable,
-    so we can hash the runnable before running it.
+    Keep an Internal Action that records the arguments evaluated from a Action,
+    so we can hash the Action before running it.
 
-    Keep a pointer to the original runnable as it's unnecessary to copy it.
+    Keep a pointer to the original Action as it's unnecessary to copy it.
     """
-    def __init__(self, runnable: Runnable, arguments: dict[str, Any]):
-        self.runnable = runnable
+    def __init__(self, action: Action, arguments: dict[str, Any]):
+        self.action = action
         self.arguments = arguments
 
     @property
     def location(self):
-        return self.runnable.location
+        return self.action.location
 
     def hash(self, ctx: Context, hash_function: StringHashFunction):
-        assert hasattr(self.runnable, "hash")
-        assert callable(self.runnable.hash)
+        assert hasattr(self.action, "hash")
+        assert callable(self.action.hash)
 
-        return self.runnable.hash(ctx=ctx, arguments=self.arguments, hash_function=hash_function)
+        return self.action.hash(ctx=ctx, arguments=self.arguments, hash_function=hash_function)
 
     def __call__(self, ctx, target: "EvaluatedTarget") -> CommandOutput:
 
-        if getattr(self.runnable, "run_with_arguments", None):
-            return self.runnable.run_with_arguments(ctx, target, self.arguments)
+        if getattr(self.action, "run_with_arguments", None):
+            return self.action.run_with_arguments(ctx, target, self.arguments)
         else:
-            return self.runnable(ctx, target)
+            return self.action(ctx, target)
 
     def __repr__(self):
-        return f"InternalRunnable({self.runnable!r}, {self.arguments})"
+        return f"InternalAction({self.action!r}, {self.arguments})"
 
 
 class Hasher:
-    def __init__(self, type=hashlib.shake_256):
-        self._hash: hashlib.shake_256 = type()
+    def __init__(self, type=HASH_FUNCTION):
+        self._hash = type()
 
     def update(self, string: str):
         self._hash.update(string.encode("ascii"))
 
     def hex_digest(self, length=20):
-        return self._hash.hexdigest(length)
+        return self._hash.hexdigest() #.hexdigest(length)
 
 
 class MakexFileProtocol(Protocol):
     path: str
     checksum: str
-    enviroment_hash: str
+    environment_hash: str
+    includes: list[str]
+
+    def hash_components(self) -> list[str]:
+        ...
 
 
 @dataclass
 class EvaluatedTarget(TargetBase):
     """
     An "evaluated" target.
 
-    All the properties/attributes in this type are resolved.
+    All the properties/attributes in this type have been evaluated or are resolved.
 
     Paths are resolved to absolute. TODO: They should retain their FileLocation for debug/ui.
 
     """
     name: str
 
     # absolute path to the output of the target
     path: Path
 
     input_path: Path
 
     workspace: Workspace = None
 
+    # all inputs used (or to be used) for this target
     inputs: list[FileStatus] = None
 
+    # all outputs produced (or to be produced) for this target
     outputs: list[FileStatus] = None
 
+    output_dict: dict[Union[int, str, None], Union[FileStatus, list[FileStatus]]] = None
+
+    # TODO: inputs dictionary, "" or None is for unnamed inputs. used for evaluation of acions
+    inputs_dictionary: dict[Union[str, None], list[Path]] = None
+
+    # references to targets this target requires.
     requires: list["EvaluatedTarget"] = None
 
-    runnables: list[InternalRunnable] = None
+    actions: list[InternalAction] = None
 
     # Contains the file path and location which the target was defined.
     location: FileLocation = None
 
     makex_file: MakexFileProtocol = None
 
     cache_path: Path = None
 
     @property
     def makex_file_path(self) -> str:
+        # TODO: fix this.
         return str(self.location.path)
 
     def key(self):
-        #if self.path is None:
-        #    raise Exception(f"Evaluated path is wrong: {self!r} {self.path!r}")
-        return format_hash_key(self.name, self.location.path)
+        return format_hash_key(self.name, self.makex_file.path)
 
     def __eq__(self, other: "EvaluatedTarget"):
-        assert hasattr(other, "key")
-        assert callable(getattr(other, "key"))
-        return self.key() == other.key()
-
-        #return self.key() == other.key()
-        #return other.name == self.name and str(other.location.path) == str(self.location.path)
+        keyfunc = getattr(other, "key", None)
+        assert keyfunc is not None
+        assert callable(keyfunc)
+        return self.key() == keyfunc()
 
     def __hash__(self):
         return hash(self.key())
 
     def __repr__(self):
         return f"EvaluatedTarget(\"{self.key()}\")" #, requires={self.requires!r})"
 
@@ -176,24 +189,21 @@
             f"key:{hash_function(self.key())}",
             f"makex-file-path:{hash_function(self.makex_file_path)}",
             f"source:{hash_function(self.input_path.as_posix())}",
             f"path:{hash_function(self.path.as_posix())}",
         ]
 
         if self.makex_file:
-            # Add the checksums of the makex file and any used environment variables.
-            data.append(f"makex-file:{self.makex_file.checksum}")
-
-            if self.makex_file.enviroment_hash:
-                data.append(f"environment:{self.makex_file.enviroment_hash}")
+            # Add the checksums of the makex file, included makex files and any used environment variables.
+            data.extend(self.makex_file.hash_components())
 
-        if self.runnables:
-            for command in self.runnables:
+        if self.actions:
+            for command in self.actions:
                 data.append(
-                    f"command:{command.runnable.__class__.__name__}:{command.hash(ctx, hash_function=hash_function)}"
+                    f"command:{command.action.__class__.__name__}:{command.hash(ctx, hash_function=hash_function)}"
                 )
 
         # XXX: Run recursively.
         # XXX: We can run require.hash because we've evaluated all targets up to this one.
         if self.requires:
             for require in self.requires:
                 rehash = False
@@ -203,32 +213,38 @@
                 else:
                     requirement_hash = hash_cache.get(require.key(), None)
                     if requirement_hash is None:
                         rehash = True
                         trace("Rehashing. Not in cache. %s", require.key())
 
                 if rehash:
-                    requirement_hash = require.hash(ctx, hash_function=hash_function)
+                    requirement_hash = require.hash(
+                        ctx,
+                        hash_function=hash_function,
+                        hash_cache=hash_cache,
+                    )
+                    # XXX: not sure about this. we should have a HashCache class which does this internally.
+                    hash_cache[require.key()] = require
 
                 data.append(f"require:{requirement_hash}")
 
         if self.inputs:
             # XXX: Inputs lists can be large (find()/glob()); optimize by using Hasher.update into one value.
-            h = Hasher()
+            _hasher = hasher()
             for input in self.inputs:
                 #data.append(f"input-file:{str(input.checksum)}")
-                h.update(f"input-file:{str(input.checksum)}")
-            data.append(h.hex_digest())
+                _hasher.update(f"input-file:{str(input.checksum)}")
+            data.append(f"input-files:{_hasher.hex_digest()}")
 
         trace("Target %s hash data: %s", self.key(), data)
         return hash_function("|".join(data))
 
 
 def target_hash(data: str):
-    return hashlib.shake_256(data.encode()).hexdigest(20)
+    return HASH_FUNCTION(data.encode()).hexdigest()
 
 
 def format_hash_key(name: str, path: str):
     return f"{path}:{name}"
 
 
 class EvaluatedTargetGraph:
@@ -377,15 +393,15 @@
             graph = self.get_requires_graph(target, scope, recursive=recursive)
             yield (target, graph)
 
     def get_inputs(self, target: EvaluatedTarget, recursive=True) -> Iterable[Path]:
         """
         yields the inputs of target and required targets.
 
-        yields target.require's inputs first, then yields target's inputs
+        yields target.require's inputs first, then yields those of target's dependendencies
 
         :param target:
         :param recursive:
         :return:
         """
         for require in target.requires:
             yield from self.get_inputs(require, recursive=recursive)
```

### Comparing `makex-20240203/python/makex/ui.py` & `makex-20240401/python/makex/ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from makex.colors import (
     ColorsNames,
     NoColors,
 )
 from makex.python_script import FileLocation
 
 
-def isansitty() -> bool:
+def is_ansi_tty() -> bool:
     """
     Checks if stdout supports ANSI escape codes and is a tty.
     https://stackoverflow.com/a/75703990
     """
 
     tty = os.isatty(sys.stdout.fileno())
     term = os.environ.get("TERM", None)
@@ -43,14 +43,19 @@
 
 
 class UI:
     def __init__(self, verbosity=None, colors=NoColors):
         self.colors = colors
         self.verbosity = verbosity or 0
 
+    def warn(self, message):
+        print(
+            f"{self.colors.MAKEX}[makex]{self.colors.RESET}{self.colors.WARNING}[WARNING]{self.colors.RESET}: {message}"
+        )
+
     def error(self, message):
         print(message, file=sys.stderr)
 
     def progress(self):
         pass
 
     def progress_multijob(self, steps: dict[str, tuple[int, int]]):
```

### Comparing `makex-20240203/python/makex/workspace.py` & `makex-20240401/python/makex/workspace.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import os
 import os.path
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
 from typing import (
     Iterable,
+    Optional,
     Union,
 )
 
 from makex.configuration import (
     Configuration,
     ConfigurationFiles,
 )
@@ -154,37 +155,26 @@
         #print(f"Get workspace of {directory}")
         # find the workspace of path
         # or find a Workspace/Workspace file in path or one of its parents
         str_path = directory.as_posix()
 
         directory_parts = directory.parts
         workspace = self._get(directory_parts)
-
         if workspace is not None:
             return workspace
 
         # search upwards for a WORKSPACE file
-        # do the key matching faster by expanding directory.parts into Iterable[tuple[str,...]]
-        def iterate_parents(parts: tuple[str]) -> Iterable[tuple[str, ...]]:
-            all_parts = parts
-            i = len(parts)
-            #print(f"all parts{all_parts}")
-            while i >= 0:
-                #print(f"Yield {all_parts[:i]} {i}")
-                yield all_parts[0:i]
-                i -= 1
-
+        # do the key matching faster by expanding directory.parts into Iterable[tuple[str,...]] using _iterate_parents
         exists = os.path.exists
-        for parent_key in iterate_parents(directory_parts):
+        for parent_key in _iterate_parents(directory_parts):
             test = self._get(parent_key)
 
             if test is not None:
                 # found a workspace in parent
                 return test
-
             ## check for workspace file if we haven't
             #test = Path(*parent_key) / WORKSPACE_FILE_NAME
             if len(parent_key) == 1:
                 # we've reached the root/anchor
                 return Workspace(_find_root(directory))
 
             test_path = os.path.join(*parent_key)
@@ -193,33 +183,41 @@
             if exists(test):
                 #print(f"Workspace at exists {test}")
                 workspace_path = test_path
                 workspace = Workspace(Path(workspace_path))
                 self._cache[parent_key] = workspace
 
                 # cache everything from directory -> workspace
-                for key in iterate_parents(directory_parts):
+                for key in _iterate_parents(directory_parts):
                     if key == parent_key:
                         break
                     self._cache[key] = workspace
                 self._cache[directory.parts] = workspace
                 return workspace
             else:
                 #print(f"Does not exist at {test}")
                 continue
 
         # no workspace detected in parents, use root
         return Workspace(_find_root(directory))
 
 
+def _iterate_parents(parts: tuple[str]) -> Iterable[tuple[str, ...]]:
+    all_parts = parts
+    i = len(parts)
+    while i >= 0:
+        yield all_parts[0:i]
+        i -= 1
+
+
 def current_workspace(
     cwd,
     files: ConfigurationFiles = None,
     argument=None,
-    environment: str = None,
+    environment: Optional[Path] = None,
 ):
     iterable = detect_workspaces(
         cwd,
         files=files,
         argument=argument,
         environment=environment,
     )
@@ -245,16 +243,16 @@
 
     return Workspace(_find_root(current_workspace))
 
 
 def detect_workspaces(
     cwd: Path,
     files: ConfigurationFiles,
-    argument: Path = None,
-    environment: Path = None,
+    argument: Optional[Path] = None,
+    environment: Optional[Path] = None,
 ) -> Iterable[Detection]:
     """ Return the currently detected workspaces from the given arguments/state.
 
         - --workspace argument
         - WORKSPACE file autodetected inside one of first parent
         - WORKSPACE environment
         - makex.workspace defined in makex.toml configuration files in one of first parents
```

### Comparing `makex-20240203/python/makex/workspace_test.py` & `makex-20240401/python/makex/workspace_test.py`

 * *Files identical despite different names*

### Comparing `makex-20240203/python/makex.egg-info/PKG-INFO` & `makex-20240401/python/makex.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,35 +1,61 @@
 Metadata-Version: 2.1
 Name: makex
-Version: 20240203
+Version: 20240401
 Summary: Build tool
 Author: Nate Skulic, MetaCompany
+Keywords: build,make,automation
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: Unix
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: Topic :: Utilities
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: toml>=0.10.2
 Requires-Dist: progressbar2>=4.3.2
+Provides-Extra: build
+Requires-Dist: build; extra == "build"
+Requires-Dist: shtab; extra == "build"
+Requires-Dist: pex; extra == "build"
+Requires-Dist: nuitka; extra == "build"
+Requires-Dist: pytest; extra == "build"
+Requires-Dist: shtab; extra == "build"
 Provides-Extra: test
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov~=3.0.0; extra == "test"
 Provides-Extra: documents
 Requires-Dist: sphinx; extra == "documents"
 Requires-Dist: sphinx-better-theme; extra == "documents"
+Requires-Dist: sphinx-notfound-page; extra == "documents"
 Requires-Dist: myst-parser; extra == "documents"
 Requires-Dist: markdown-it-py[linkify,plugins]; extra == "documents"
 
 # makex
 
 <!-- heading -->
 
-Makex is a new and simplified automation tool, similar to the original [Make](https://en.wikipedia.org/wiki/Make_(software)).
+Makex is a new and simplified build and automation tool, similar to the original [Make](https://en.wikipedia.org/wiki/Make_(software)).
 
 It __*makex*__ stuff happen. 🙂
 
 <!-- features -->
 
+
+## What Makex is used for
+
+- Compiling software/applications/firmware
+- Building filesystems/trees/file archives
+- Building and deploying websites and web applications
+- Running things in a repeatable manner
+- Replacing most or all of the other build systems
+
 ## Features
 
 - Familiar Syntax
 - File Hashing and Checksums
 - Dependency Graphs
 - Caching
 - Workspaces
@@ -45,46 +71,46 @@
 - Support: [Google Groups](http://groups.google.com/group/makex) or [makex@googlegroups.com](mailto://makex@googlegroups.com)
 
 <!-- quick-start -->
 
 
 ## Quick Start
 
-- Install:
+1. Install:
 
   ```shell
   pip install makex
   ```
 
-- Define a Makex file (name it `Makexfile`):
+2. Define a Makex file (name it `Makexfile`):
 
   ```python
   #!makex
   
-  target(
+  task(
       name="hello-world",
-      runs=[
+      steps=[
           write("hello-world.txt", "Hello World!"),
   
           # or, you can use the shell, but it's not recommended:
           # shell(f"echo 'Hello World!' > {path('hello-world')}/hello-world.txt"),
       ],
       outputs=[
           "hello-world.txt",
       ],
   )
   ```
 
-- Run makex and the target:
+3. Run makex and the target:
 
   ```shell
   makex run :hello-world
   ```
  
-- A file at `_output_/hello-world/hello-world.txt` will have the following contents:
+4. A file at `_output_/hello-world/hello-world.txt` will have the following contents:
 
   ```
   Hello World!
   ```
 
 
 ## Limitations
```

### Comparing `makex-20240203/python/makex.egg-info/SOURCES.txt` & `makex-20240401/python/makex.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 README.md
 pyproject.toml
+python/benchmarks/hashing_benchmark_test.py
 python/makex/__main__.py
 python/makex/_logging.py
 python/makex/_shtab.py
 python/makex/api.py
 python/makex/build_path.py
 python/makex/colors.py
 python/makex/configuration.py
 python/makex/constants.py
 python/makex/context.py
 python/makex/errors.py
 python/makex/executor.py
 python/makex/executor_test.py
 python/makex/file_checksum.py
 python/makex/file_checksum_test.py
+python/makex/file_cloning.py
+python/makex/file_cloning_test.py
 python/makex/file_system.py
 python/makex/flags.py
-python/makex/make_file.py
-python/makex/makefile_test.py
+python/makex/makex_file.py
+python/makex/makex_file_parser.py
+python/makex/makex_file_parser_test.py
+python/makex/makex_file_types.py
 python/makex/metadata.py
 python/makex/metadata_file.py
 python/makex/metadata_sqlite.py
 python/makex/metadata_sqlite_test.py
 python/makex/metadata_test.py
 python/makex/patterns.py
 python/makex/patterns_test.py
 python/makex/protocols.py
 python/makex/python_script.py
-python/makex/reflink.py
-python/makex/reflink_test.py
 python/makex/run.py
 python/makex/target.py
 python/makex/ui.py
 python/makex/version.py
 python/makex/workspace.py
 python/makex/workspace_test.py
 python/makex.egg-info/PKG-INFO
 python/makex.egg-info/SOURCES.txt
 python/makex.egg-info/dependency_links.txt
 python/makex.egg-info/entry_points.txt
 python/makex.egg-info/requires.txt
 python/makex.egg-info/top_level.txt
 python/makex/data/completions/makex.bash
 python/makex/data/completions/makex.zsh
+python/makex/integrations/intellij.py
+python/makex/integrations/vscode.py
 python/makex/platform_object/__init__.py
 python/makex/platform_object/platform_object.py
 python/makex/platform_object/platform_test.py
```

