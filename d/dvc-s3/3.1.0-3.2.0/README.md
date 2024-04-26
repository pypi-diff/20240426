# Comparing `tmp/dvc-s3-3.1.0.tar.gz` & `tmp/dvc_s3-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dvc-s3-3.1.0.tar", last modified: Mon Mar  4 09:38:19 2024, max compression
+gzip compressed data, was "dvc_s3-3.2.0.tar", last modified: Fri Apr 26 13:23:22 2024, max compression
```

## Comparing `dvc-s3-3.1.0.tar` & `dvc_s3-3.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:38:19.888428 dvc-s3-3.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/.cruft.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:38:19.884428 dvc-s3-3.1.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:38:19.888428 dvc-s3-3.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/.github/workflows/benchmarks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/.github/workflows/tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/.github/workflows/update-template.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-04 09:38:19.888428 dvc-s3-3.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      193 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:38:19.888428 dvc-s3-3.1.0/dvc_s3/
--rw-r--r--   0 runner    (1001) docker     (127)     9059 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/dvc_s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      411 2024-03-04 09:38:19.000000 dvc-s3-3.1.0/dvc_s3/_dvc_s3_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:38:19.888428 dvc-s3-3.1.0/dvc_s3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/dvc_s3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/dvc_s3/tests/benchmarks.py
--rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/dvc_s3/tests/cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/dvc_s3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/dvc_s3/tests/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/dvc_s3/tests/test_dvc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/dvc_s3/tests/test_s3.py
--rw-r--r--   0 runner    (1001) docker     (127)      728 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/dvc_s3/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 09:38:19.888428 dvc-s3-3.1.0/dvc_s3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-03-04 09:38:19.000000 dvc-s3-3.1.0/dvc_s3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-04 09:38:19.000000 dvc-s3-3.1.0/dvc_s3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 09:38:19.000000 dvc-s3-3.1.0/dvc_s3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-03-04 09:38:19.000000 dvc-s3-3.1.0/dvc_s3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-04 09:38:19.000000 dvc-s3-3.1.0/dvc_s3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-03-04 09:38:09.000000 dvc-s3-3.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 09:38:19.888428 dvc-s3-3.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:22.200534 dvc_s3-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/.cruft.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:22.196534 dvc_s3-3.2.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:22.196534 dvc_s3-3.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/.github/workflows/benchmarks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/.github/workflows/update-template.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-26 13:23:22.200534 dvc_s3-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      193 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:22.196534 dvc_s3-3.2.0/dvc_s3/
+-rw-r--r--   0 runner    (1001) docker     (127)     9124 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/dvc_s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-26 13:23:22.000000 dvc_s3-3.2.0/dvc_s3/_dvc_s3_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:22.196534 dvc_s3-3.2.0/dvc_s3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/dvc_s3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/dvc_s3/tests/benchmarks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3882 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/dvc_s3/tests/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/dvc_s3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1348 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/dvc_s3/tests/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/dvc_s3/tests/test_dvc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/dvc_s3/tests/test_s3.py
+-rw-r--r--   0 runner    (1001) docker     (127)      728 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/dvc_s3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 13:23:22.200534 dvc_s3-3.2.0/dvc_s3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-26 13:23:22.000000 dvc_s3-3.2.0/dvc_s3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-26 13:23:22.000000 dvc_s3-3.2.0/dvc_s3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 13:23:22.000000 dvc_s3-3.2.0/dvc_s3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-26 13:23:22.000000 dvc_s3-3.2.0/dvc_s3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 13:23:22.000000 dvc_s3-3.2.0/dvc_s3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3057 2024-04-26 13:23:09.000000 dvc_s3-3.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 13:23:22.200534 dvc_s3-3.2.0/setup.cfg
```

### Comparing `dvc-s3-3.1.0/.github/workflows/benchmarks.yaml` & `dvc_s3-3.2.0/.github/workflows/benchmarks.yaml`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/.github/workflows/release.yaml` & `dvc_s3-3.2.0/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/.github/workflows/tests.yaml` & `dvc_s3-3.2.0/.github/workflows/tests.yaml`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/.github/workflows/update-template.yaml` & `dvc_s3-3.2.0/.github/workflows/update-template.yaml`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/.gitignore` & `dvc_s3-3.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/.pre-commit-config.yaml` & `dvc_s3-3.2.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,21 @@
       - id: no rej
         name: Check for .rej files
         entry: .rej files found, fix conflicts from these rejected files.
         language: fail
         files: \.rej$
     repo: local
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: 'v0.3.0'
+    rev: 'v0.4.1'
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
       - id: ruff-format
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-toml
       - id: check-yaml
   - hooks:
       - id: codespell
         args:
           - --ignore-words-list
```

### Comparing `dvc-s3-3.1.0/LICENSE` & `dvc_s3-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/PKG-INFO` & `dvc_s3-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-s3
-Version: 3.1.0
+Version: 3.2.0
 Summary: s3 plugin for dvc
 Author-email: Iterative <support@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-s3
 Keywords: dvc,s3
@@ -19,15 +19,15 @@
 License-File: LICENSE
 Requires-Dist: dvc
 Requires-Dist: s3fs>=2023.6.0
 Requires-Dist: aiobotocore[boto3]>=2.5.0
 Requires-Dist: flatten_dict<1,>=0.4.1
 Provides-Extra: dev
 Requires-Dist: dvc-s3[tests]; extra == "dev"
-Requires-Dist: mypy==1.8.0; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
 Provides-Extra: tests
 Requires-Dist: dvc[testing]; extra == "tests"
 Requires-Dist: pytest<9,>=7; extra == "tests"
 Requires-Dist: pytest-cov>=4.1.0; extra == "tests"
 Requires-Dist: pytest-xdist>=3.2; extra == "tests"
 Requires-Dist: pytest-servers[s3]>=0.4.0; extra == "tests"
```

### Comparing `dvc-s3-3.1.0/dvc_s3/__init__.py` & `dvc_s3-3.2.0/dvc_s3/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,14 +163,15 @@
         login_info["key"] = config.get("access_key_id")
         login_info["secret"] = config.get("secret_access_key")
         login_info["token"] = config.get("session_token")
 
         # session configuration
         login_info["profile"] = config.get("profile")
         login_info["use_ssl"] = config.get("use_ssl", True)
+        login_info["anon"] = config.get("allow_anonymous_login")
 
         # extra client configuration
         client = login_info["client_kwargs"]
         client["region_name"] = config.get("region")
         client["endpoint_url"] = config.get("endpointurl")
         client["verify"] = config.get("ssl_verify")
```

### Comparing `dvc-s3-3.1.0/dvc_s3/tests/cloud.py` & `dvc_s3-3.2.0/dvc_s3/tests/cloud.py`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/dvc_s3/tests/fixtures.py` & `dvc_s3-3.2.0/dvc_s3/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/dvc_s3/tests/test_dvc.py` & `dvc_s3-3.2.0/dvc_s3/tests/test_dvc.py`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/dvc_s3/tests/test_s3.py` & `dvc_s3-3.2.0/dvc_s3/tests/test_s3.py`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/dvc_s3/tests/test_utils.py` & `dvc_s3-3.2.0/dvc_s3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/dvc_s3.egg-info/PKG-INFO` & `dvc_s3-3.2.0/dvc_s3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dvc-s3
-Version: 3.1.0
+Version: 3.2.0
 Summary: s3 plugin for dvc
 Author-email: Iterative <support@dvc.org>
 Maintainer-email: Iterative <support@dvc.org>
 License: Apache License 2.0
 Project-URL: Documentation, https://dvc.org/doc
 Project-URL: Source, https://github.com/iterative/dvc-s3
 Keywords: dvc,s3
@@ -19,15 +19,15 @@
 License-File: LICENSE
 Requires-Dist: dvc
 Requires-Dist: s3fs>=2023.6.0
 Requires-Dist: aiobotocore[boto3]>=2.5.0
 Requires-Dist: flatten_dict<1,>=0.4.1
 Provides-Extra: dev
 Requires-Dist: dvc-s3[tests]; extra == "dev"
-Requires-Dist: mypy==1.8.0; extra == "dev"
+Requires-Dist: mypy==1.9.0; extra == "dev"
 Provides-Extra: tests
 Requires-Dist: dvc[testing]; extra == "tests"
 Requires-Dist: pytest<9,>=7; extra == "tests"
 Requires-Dist: pytest-cov>=4.1.0; extra == "tests"
 Requires-Dist: pytest-xdist>=3.2; extra == "tests"
 Requires-Dist: pytest-servers[s3]>=0.4.0; extra == "tests"
```

### Comparing `dvc-s3-3.1.0/dvc_s3.egg-info/SOURCES.txt` & `dvc_s3-3.2.0/dvc_s3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dvc-s3-3.1.0/pyproject.toml` & `dvc_s3-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     "aiobotocore[boto3]>=2.5.0",
     "flatten_dict>=0.4.1,<1",
 ]
 
 [project.optional-dependencies]
 dev = [
     "dvc-s3[tests]",
-    "mypy==1.8.0",
+    "mypy==1.9.0",
 ]
 tests = [
     "dvc[testing]",
     "pytest>=7,<9",
     "pytest-cov>=4.1.0",
     "pytest-xdist>=3.2",
     "pytest-servers[s3]>=0.4.0",
```

