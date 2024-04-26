# Comparing `tmp/classy_config-0.5.1.tar.gz` & `tmp/classy_config-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "classy_config-0.5.1.tar", max compression
+gzip compressed data, was "classy_config-0.6.0.tar", max compression
```

## Comparing `classy_config-0.5.1.tar` & `classy_config-0.6.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1061 2023-11-09 22:10:03.168472 classy_config-0.5.1/LICENSE
--rw-r--r--   0        0        0     2463 2023-11-09 22:10:03.168472 classy_config-0.5.1/README.md
--rw-r--r--   0        0        0      177 2023-11-09 22:10:03.168472 classy_config-0.5.1/classy_config/__init__.py
--rw-r--r--   0        0        0      819 2023-11-09 22:10:03.168472 classy_config-0.5.1/classy_config/_util.py
--rw-r--r--   0        0        0     2633 2023-11-09 22:10:03.168472 classy_config-0.5.1/classy_config/config.py
--rw-r--r--   0        0        0       64 2023-11-09 22:10:03.168472 classy_config-0.5.1/classy_config/loader/__init__.py
--rw-r--r--   0        0        0      993 2023-11-09 22:10:03.168472 classy_config-0.5.1/classy_config/loader/auto_loader.py
--rw-r--r--   0        0        0      580 2023-11-09 22:10:03.168472 classy_config-0.5.1/classy_config/loader/env_loader.py
--rw-r--r--   0        0        0      391 2023-11-09 22:10:03.168472 classy_config-0.5.1/classy_config/loader/json_loader.py
--rw-r--r--   0        0        0      441 2023-11-09 22:10:03.168472 classy_config-0.5.1/classy_config/loader/loader.py
--rw-r--r--   0        0        0      251 2023-11-09 22:10:03.168472 classy_config-0.5.1/classy_config/loader/toml_loader.py
--rw-r--r--   0        0        0     1000 2023-11-09 22:10:14.244508 classy_config-0.5.1/pyproject.toml
--rw-r--r--   0        0        0     3392 1970-01-01 00:00:00.000000 classy_config-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1061 2024-04-26 10:36:49.145358 classy_config-0.6.0/LICENSE
+-rw-r--r--   0        0        0     2463 2024-04-26 10:36:49.145358 classy_config-0.6.0/README.md
+-rw-r--r--   0        0        0      177 2024-04-26 10:36:49.145358 classy_config-0.6.0/classy_config/__init__.py
+-rw-r--r--   0        0        0      819 2024-04-26 10:36:49.145358 classy_config-0.6.0/classy_config/_util.py
+-rw-r--r--   0        0        0     2633 2024-04-26 10:36:49.145358 classy_config-0.6.0/classy_config/config.py
+-rw-r--r--   0        0        0       64 2024-04-26 10:36:49.149358 classy_config-0.6.0/classy_config/loader/__init__.py
+-rw-r--r--   0        0        0      993 2024-04-26 10:36:49.149358 classy_config-0.6.0/classy_config/loader/auto_loader.py
+-rw-r--r--   0        0        0      580 2024-04-26 10:36:49.149358 classy_config-0.6.0/classy_config/loader/env_loader.py
+-rw-r--r--   0        0        0      391 2024-04-26 10:36:49.149358 classy_config-0.6.0/classy_config/loader/json_loader.py
+-rw-r--r--   0        0        0      441 2024-04-26 10:36:49.149358 classy_config-0.6.0/classy_config/loader/loader.py
+-rw-r--r--   0        0        0      251 2024-04-26 10:36:49.149358 classy_config-0.6.0/classy_config/loader/toml_loader.py
+-rw-r--r--   0        0        0     1001 2024-04-26 10:37:01.681406 classy_config-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3393 1970-01-01 00:00:00.000000 classy_config-0.6.0/PKG-INFO
```

### Comparing `classy_config-0.5.1/LICENSE` & `classy_config-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `classy_config-0.5.1/README.md` & `classy_config-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `classy_config-0.5.1/classy_config/_util.py` & `classy_config-0.6.0/classy_config/_util.py`

 * *Files identical despite different names*

### Comparing `classy_config-0.5.1/classy_config/config.py` & `classy_config-0.6.0/classy_config/config.py`

 * *Files identical despite different names*

### Comparing `classy_config-0.5.1/classy_config/loader/auto_loader.py` & `classy_config-0.6.0/classy_config/loader/auto_loader.py`

 * *Files identical despite different names*

### Comparing `classy_config-0.5.1/classy_config/loader/env_loader.py` & `classy_config-0.6.0/classy_config/loader/env_loader.py`

 * *Files identical despite different names*

### Comparing `classy_config-0.5.1/pyproject.toml` & `classy_config-0.6.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 [tool.poetry]
 name = "classy_config"
-version = "0.5.1"
+version = "0.6.0"
 description = "ClassyConfig is a Python3 package aiming to remove the need for a config.py or settings.py file."
 readme = "README.md"
 repository = "https://github.com/GDWR/classy-config"
 authors = ["GDWR <gregory.dwr@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = "^1.9.0"
-typing-inspect = ">=0.7.1,<0.9.0"
+typing-inspect = ">=0.7.1,<0.10.0"
 toml = "^0.10.2"
 python-dotenv = ">=0.20,<1.1"
 
 [tool.poetry.dev-dependencies]
 pyright = "^1.1.314"
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 flake8 = "^5.0.4"
-Sphinx = "^5.3.0"
+Sphinx = "^6.2.1"
 sphinxcontrib-napoleon = "^0.7"
 flake8-annotations = "^2.9.1"
 flake8-bandit = "^4.1.1"
 flake8-bugbear = "^23.3.12"
 flake8-docstrings = "^1.7.0"
 flake8-import-order = "^0.18.2"
 flake8-string-format = "^0.3.0"
 pep8-naming = "^0.13.3"
-furo = "^2022.12.7"
+furo = "^2023.3.27"
 
 [tool.pyright]
 include = ["classy_config"]
 exclude = [
     "**/__pycache__",
 ]
```

### Comparing `classy_config-0.5.1/PKG-INFO` & `classy_config-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: classy_config
-Version: 0.5.1
+Version: 0.6.0
 Summary: ClassyConfig is a Python3 package aiming to remove the need for a config.py or settings.py file.
 Home-page: https://github.com/GDWR/classy-config
 License: MIT
 Author: GDWR
 Author-email: gregory.dwr@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: pydantic (>=1.9.0,<2.0.0)
 Requires-Dist: python-dotenv (>=0.20,<1.1)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
-Requires-Dist: typing-inspect (>=0.7.1,<0.9.0)
+Requires-Dist: typing-inspect (>=0.7.1,<0.10.0)
 Project-URL: Repository, https://github.com/GDWR/classy-config
 Description-Content-Type: text/markdown
 
 <div align="center">
     <img align="center" src="https://raw.githubusercontent.com/GDWR/classy-config/main/docs/favicon.ico" alt="ClassyConfig Logo">
     <h1 align="center">ClassyConfig</h1>
 </div>
```

