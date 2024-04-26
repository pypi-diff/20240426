# Comparing `tmp/layered_config_tree-1.0.1.tar.gz` & `tmp/layered_config_tree-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layered_config_tree-1.0.1.tar", last modified: Tue Apr 16 19:57:38 2024, max compression
+gzip compressed data, was "layered_config_tree-1.0.2.tar", last modified: Fri Apr 26 21:35:52 2024, max compression
```

## Comparing `layered_config_tree-1.0.1.tar` & `layered_config_tree-1.0.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.698656 layered_config_tree-1.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.github/workflows/update_readme.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-16 19:57:38.694656 layered_config_tree-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/docs/source/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/docs/source/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/docs/source/_static/style.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.690656 layered_config_tree-1.0.1/docs/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/docs/source/_templates/layout.html
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/python_versions.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:57:38.698656 layered_config_tree-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.686656 layered_config_tree-1.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.694656 layered_config_tree-1.0.1/src/layered_config_tree/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/src/layered_config_tree/__about__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/src/layered_config_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      991 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/src/layered_config_tree/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    19980 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/src/layered_config_tree/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.694656 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:57:34.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-16 19:57:38.000000 layered_config_tree-1.0.1/src/layered_config_tree.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.694656 layered_config_tree-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/test_basic_functionality.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:57:38.694656 layered_config_tree-1.0.1/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/test_data/mock_model_specification.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/test_data/mock_model_specification.yml
--rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/tests/test_ingestion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-16 19:57:25.000000 layered_config_tree-1.0.1/update_readme.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (127)      821 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.github/workflows/update_readme.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      842 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      579 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/docs/source/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/docs/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/docs/source/_static/style.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/docs/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/docs/source/_templates/layout.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/python_versions.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3225 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.442951 layered_config_tree-1.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.446951 layered_config_tree-1.0.2/src/layered_config_tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/src/layered_config_tree/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/src/layered_config_tree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      998 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/src/layered_config_tree/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19980 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/src/layered_config_tree/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2274 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 21:35:48.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 21:35:52.000000 layered_config_tree-1.0.2/src/layered_config_tree.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17155 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/test_basic_functionality.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 21:35:52.450951 layered_config_tree-1.0.2/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/test_data/mock_model_specification.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/test_data/mock_model_specification.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/tests/test_ingestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-26 21:35:42.000000 layered_config_tree-1.0.2/update_readme.py
```

### Comparing `layered_config_tree-1.0.1/.github/pull_request_template.md` & `layered_config_tree-1.0.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/.github/workflows/build.yml` & `layered_config_tree-1.0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/.github/workflows/deploy.yml` & `layered_config_tree-1.0.2/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/.github/workflows/update_readme.yml` & `layered_config_tree-1.0.2/.github/workflows/update_readme.yml`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/.gitignore` & `layered_config_tree-1.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/.readthedocs.yaml` & `layered_config_tree-1.0.2/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/CODE_OF_CONDUCT.rst` & `layered_config_tree-1.0.2/CODE_OF_CONDUCT.rst`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/CONTRIBUTING.rst` & `layered_config_tree-1.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/LICENSE.txt` & `layered_config_tree-1.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/PKG-INFO` & `layered_config_tree-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layered_config_tree
-Version: 1.0.1
+Version: 1.0.2
 Summary: Layered Config Tree is a configuration structure which supports cascading layers.
 Home-page: https://github.com/ihmeuw/layered_config_tree
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `layered_config_tree-1.0.1/README.rst` & `layered_config_tree-1.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/docs/Makefile` & `layered_config_tree-1.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/docs/source/conf.py` & `layered_config_tree-1.0.2/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/setup.py` & `layered_config_tree-1.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/src/layered_config_tree/exceptions.py` & `layered_config_tree-1.0.2/src/layered_config_tree/exceptions.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from typing import Any, Optional
 
 
 class ConfigurationError(Exception):
     """Base class for configuration errors."""
 
-    def __init__(self, message: str, value_name: Optional[str]):
+    def __init__(self, message: str, value_name: Optional[str] = None):
         super().__init__(message)
         self.value_name = value_name
 
 
 class ConfigurationKeyError(ConfigurationError, KeyError):
     """Error raised when a configuration lookup fails."""
```

### Comparing `layered_config_tree-1.0.1/src/layered_config_tree/main.py` & `layered_config_tree-1.0.2/src/layered_config_tree/main.py`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/src/layered_config_tree.egg-info/PKG-INFO` & `layered_config_tree-1.0.2/src/layered_config_tree.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layered_config_tree
-Version: 1.0.1
+Version: 1.0.2
 Summary: Layered Config Tree is a configuration structure which supports cascading layers.
 Home-page: https://github.com/ihmeuw/layered_config_tree
 Author: The vivarium developers
 Author-email: vivarium.dev@gmail.com
 License: BSD-3-Clause
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

### Comparing `layered_config_tree-1.0.1/src/layered_config_tree.egg-info/SOURCES.txt` & `layered_config_tree-1.0.2/src/layered_config_tree.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/tests/conftest.py` & `layered_config_tree-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/tests/test_basic_functionality.py` & `layered_config_tree-1.0.2/tests/test_basic_functionality.py`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/tests/test_ingestion.py` & `layered_config_tree-1.0.2/tests/test_ingestion.py`

 * *Files identical despite different names*

### Comparing `layered_config_tree-1.0.1/update_readme.py` & `layered_config_tree-1.0.2/update_readme.py`

 * *Files identical despite different names*

