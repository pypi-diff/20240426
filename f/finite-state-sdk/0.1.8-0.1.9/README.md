# Comparing `tmp/finite_state_sdk-0.1.8.tar.gz` & `tmp/finite_state_sdk-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finite_state_sdk-0.1.8.tar", max compression
+gzip compressed data, was "finite_state_sdk-0.1.9.tar", max compression
```

## Comparing `finite_state_sdk-0.1.8.tar` & `finite_state_sdk-0.1.9.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1061 2024-03-29 20:05:40.406290 finite_state_sdk-0.1.8/LICENSE
--rw-r--r--   0        0        0     2053 2024-03-29 20:05:40.406388 finite_state_sdk-0.1.8/README.md
--rw-r--r--   0        0        0    97803 2024-04-18 17:26:48.715381 finite_state_sdk-0.1.8/finite_state_sdk/__init__.py
--rw-r--r--   0        0        0    24623 2024-04-10 18:42:22.532040 finite_state_sdk-0.1.8/finite_state_sdk/queries.py
--rw-r--r--   0        0        0     2634 2024-04-10 18:42:22.532375 finite_state_sdk-0.1.8/finite_state_sdk/token_cache.py
--rw-r--r--   0        0        0     3016 2024-04-18 17:44:52.926353 finite_state_sdk-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4686 1970-01-01 00:00:00.000000 finite_state_sdk-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1061 2023-12-15 12:24:45.214803 finite_state_sdk-0.1.9/LICENSE
+-rw-r--r--   0        0        0     2220 2024-04-26 18:55:09.219325 finite_state_sdk-0.1.9/README.md
+-rw-r--r--   0        0        0    97803 2024-04-18 18:48:28.241387 finite_state_sdk-0.1.9/finite_state_sdk/__init__.py
+-rw-r--r--   0        0        0    24623 2024-04-18 18:48:28.242347 finite_state_sdk-0.1.9/finite_state_sdk/queries.py
+-rw-r--r--   0        0        0     2634 2024-04-18 18:48:28.242711 finite_state_sdk-0.1.9/finite_state_sdk/token_cache.py
+-rw-r--r--   0        0        0     2946 2024-04-26 18:55:09.234040 finite_state_sdk-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4702 1970-01-01 00:00:00.000000 finite_state_sdk-0.1.9/PKG-INFO
```

### Comparing `finite_state_sdk-0.1.8/LICENSE` & `finite_state_sdk-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `finite_state_sdk-0.1.8/README.md` & `finite_state_sdk-0.1.9/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -29,18 +29,36 @@
 
 ```
 import finite_state_sdk
 ```
 
 ## Generating the docs
 
+### Setting docs generation project
+
+`docs-generation` folder is the python project to generate html documentation.
+
+`./docs-generation/pyproject.toml` is the Poetry file project. It should run with python 3.9 or up.
+
+Should run once the following commands. This is an example with pyenv and python 3.11.
+
+```bash
+cd docs-generation
+pyenv local 3.11
+poetry env use 3.11
+poetry install
+```
+
+### Generation docs.
+
+From project root folder.
+
 ```bash
-pip3 install pdoc
 export VERSION=0.0.4
-pdoc -o docs -d google --logo "https://camo.githubusercontent.com/ea2191106c0aa7006f669bef130bf089bb3fedc0463bcecebeabbefd6b4362ad/68747470733a2f2f66696e69746573746174652e696f2f68732d66732f68756266732f46532d4c6f676f2d46696e616c2d30312e706e67" -t ./docs-template ./finite_state_sdk
+./scripts/generate-docs.sh
 ```
 
 # Finite State API
 
 For more information about Finite State's APIs, see: [https://docs.finitestate.io](https://docs.finitestate.io).
 
 Our teams are working to add additional programming language and package manager support for Finite State SDKs.
```

### Comparing `finite_state_sdk-0.1.8/finite_state_sdk/__init__.py` & `finite_state_sdk-0.1.9/finite_state_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `finite_state_sdk-0.1.8/finite_state_sdk/queries.py` & `finite_state_sdk-0.1.9/finite_state_sdk/queries.py`

 * *Files identical despite different names*

### Comparing `finite_state_sdk-0.1.8/finite_state_sdk/token_cache.py` & `finite_state_sdk-0.1.9/finite_state_sdk/token_cache.py`

 * *Files identical despite different names*

### Comparing `finite_state_sdk-0.1.8/pyproject.toml` & `finite_state_sdk-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,83 +1,78 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "finite-state-sdk"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
     "Finite State, Inc. <developer-tools@finitestate.io>"
 ]
 maintainers = [
     "Finite State, Inc. <developer-tools@finitestate.io>"
 ]
 repository = "https://www.github.com/FiniteStateInc/finite-state-sdk-python"
 homepage = "https://github.com/FiniteStateInc/finite-state-sdk-python"
 description = "The official Finite State Python SDK."
 readme = "README.md"
 license = "MIT"
 classifiers = [
+    "Programming Language :: Python :: 3.8.1",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = "^3.8.1"
 bleach = "^6.1.0"
 build = "^1.2.1"
 certifi = "^2024.2.2"
 charset-normalizer = "^3.2.0"
 cyclonedx-bom = "==3.11.7"
 cyclonedx-python-lib = "==3.1.5"
-docutils = "^0.21.1"
 idna = "^3.4"
 importlib-metadata = "^7.1.0"
 jaraco-classes = "^3.3.0"
 Jinja2 = "^3.1.2"
 keyring = "^25.1.0"
 markdown-it-py = "^3.0.0"
 MarkupSafe = "^2.1.3"
 mdurl = "^0.1.2"
 more-itertools = "^10.2.0"
 packageurl-python = "^0.15.0"
 packaging = "^24.0"
-pdoc = "^14.0.0"
 pip-requirements-parser = "^32.0.1"
 pkginfo = "^1.9.6"
 Pygments = "^2.15.1"
 pyparsing = "^3.1.0"
 pyproject_hooks = "^1.0.0"
-readme-renderer = "^43.0"
 requests = "^2.31.0"
 requests-toolbelt = "^1.0.0"
 rfc3986 = "^2.0.0"
 six = "^1.16.0"
 sortedcontainers = "^2.4.0"
 toml = "^0.10.2"
 tomli = "^2.0.1"
-twine = "^5.0.0"
-urllib3 = "^2.0.3"
 webencodings = "^0.5.1"
 zipp = "^3.16.2"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.9.1"
 flake8 = "^6.1.0"
 isort = "^5.12.0"
-libcst = "^1.0.1"
 rich = "^13.5.2"
 typer = "^0.9.0"
 pytest = "^7.4.2"
 pytest-cov = "^3.0.0"
 flake8-pyproject = "^1.2.3"
 darker = "^1.7.2"
```

### Comparing `finite_state_sdk-0.1.8/PKG-INFO` & `finite_state_sdk-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,64 +1,60 @@
 Metadata-Version: 2.1
 Name: finite-state-sdk
-Version: 0.1.8
+Version: 0.1.9
 Summary: The official Finite State Python SDK.
 Home-page: https://github.com/FiniteStateInc/finite-state-sdk-python
 License: MIT
 Author: Finite State, Inc.
 Author-email: developer-tools@finitestate.io
 Maintainer: Finite State, Inc.
 Maintainer-email: developer-tools@finitestate.io
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.8.1
 Classifier: Topic :: Security
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: Jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: MarkupSafe (>=2.1.3,<3.0.0)
 Requires-Dist: Pygments (>=2.15.1,<3.0.0)
 Requires-Dist: bleach (>=6.1.0,<7.0.0)
 Requires-Dist: build (>=1.2.1,<2.0.0)
 Requires-Dist: certifi (>=2024.2.2,<2025.0.0)
 Requires-Dist: charset-normalizer (>=3.2.0,<4.0.0)
 Requires-Dist: cyclonedx-bom (==3.11.7)
 Requires-Dist: cyclonedx-python-lib (==3.1.5)
-Requires-Dist: docutils (>=0.21.1,<0.22.0)
 Requires-Dist: idna (>=3.4,<4.0)
 Requires-Dist: importlib-metadata (>=7.1.0,<8.0.0)
 Requires-Dist: jaraco-classes (>=3.3.0,<4.0.0)
 Requires-Dist: keyring (>=25.1.0,<26.0.0)
 Requires-Dist: markdown-it-py (>=3.0.0,<4.0.0)
 Requires-Dist: mdurl (>=0.1.2,<0.2.0)
 Requires-Dist: more-itertools (>=10.2.0,<11.0.0)
 Requires-Dist: packageurl-python (>=0.15.0,<0.16.0)
 Requires-Dist: packaging (>=24.0,<25.0)
-Requires-Dist: pdoc (>=14.0.0,<15.0.0)
 Requires-Dist: pip-requirements-parser (>=32.0.1,<33.0.0)
 Requires-Dist: pkginfo (>=1.9.6,<2.0.0)
 Requires-Dist: pyparsing (>=3.1.0,<4.0.0)
 Requires-Dist: pyproject_hooks (>=1.0.0,<2.0.0)
-Requires-Dist: readme-renderer (>=43.0,<44.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Requires-Dist: rfc3986 (>=2.0.0,<3.0.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Requires-Dist: sortedcontainers (>=2.4.0,<3.0.0)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
-Requires-Dist: twine (>=5.0.0,<6.0.0)
-Requires-Dist: urllib3 (>=2.0.3,<3.0.0)
 Requires-Dist: webencodings (>=0.5.1,<0.6.0)
 Requires-Dist: zipp (>=3.16.2,<4.0.0)
 Project-URL: Repository, https://www.github.com/FiniteStateInc/finite-state-sdk-python
 Description-Content-Type: text/markdown
 
 <p align="center">
   <img src="https://finitestate.io/hs-fs/hubfs/FS-Logo-Final-01.png" />
@@ -91,18 +87,36 @@
 
 ```
 import finite_state_sdk
 ```
 
 ## Generating the docs
 
+### Setting docs generation project
+
+`docs-generation` folder is the python project to generate html documentation.
+
+`./docs-generation/pyproject.toml` is the Poetry file project. It should run with python 3.9 or up.
+
+Should run once the following commands. This is an example with pyenv and python 3.11.
+
+```bash
+cd docs-generation
+pyenv local 3.11
+poetry env use 3.11
+poetry install
+```
+
+### Generation docs.
+
+From project root folder.
+
 ```bash
-pip3 install pdoc
 export VERSION=0.0.4
-pdoc -o docs -d google --logo "https://camo.githubusercontent.com/ea2191106c0aa7006f669bef130bf089bb3fedc0463bcecebeabbefd6b4362ad/68747470733a2f2f66696e69746573746174652e696f2f68732d66732f68756266732f46532d4c6f676f2d46696e616c2d30312e706e67" -t ./docs-template ./finite_state_sdk
+./scripts/generate-docs.sh
 ```
 
 # Finite State API
 
 For more information about Finite State's APIs, see: [https://docs.finitestate.io](https://docs.finitestate.io).
 
 Our teams are working to add additional programming language and package manager support for Finite State SDKs.
```

