# Comparing `tmp/pre_commit_update-0.3.0.tar.gz` & `tmp/pre_commit_update-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pre_commit_update-0.3.0.tar", max compression
+gzip compressed data, was "pre_commit_update-0.3.1.tar", max compression
```

## Comparing `pre_commit_update-0.3.0.tar` & `pre_commit_update-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1058 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/LICENSE
--rw-r--r--   0        0        0     6689 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/README.md
--rw-r--r--   0        0        0     1660 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-11 15:53:44.498016 pre_commit_update-0.3.0/src/pre_commit_update/__init__.py
--rw-r--r--   0        0        0     3167 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/cli.py
--rw-r--r--   0        0        0      229 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/managers/__init__.py
--rw-r--r--   0        0        0      685 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/managers/env.py
--rw-r--r--   0        0        0     3116 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/managers/message.py
--rw-r--r--   0        0        0     4526 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/managers/repo.py
--rw-r--r--   0        0        0      800 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/managers/yaml.py
--rw-r--r--   0        0        0        0 2022-04-01 23:18:32.000000 pre_commit_update-0.3.0/src/pre_commit_update/py.typed
--rw-r--r--   0        0        0     2151 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/repo.py
--rw-r--r--   0        0        0      759 2024-04-18 17:00:48.849180 pre_commit_update-0.3.0/src/pre_commit_update/utils.py
--rw-r--r--   0        0        0     8233 1970-01-01 00:00:00.000000 pre_commit_update-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/LICENSE
+-rw-r--r--   0        0        0     6594 2024-04-26 20:49:14.183951 pre_commit_update-0.3.1/README.md
+-rw-r--r--   0        0        0     1675 2024-04-26 20:45:38.009532 pre_commit_update-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/__init__.py
+-rw-r--r--   0        0        0     3167 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/cli.py
+-rw-r--r--   0        0        0      229 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/managers/__init__.py
+-rw-r--r--   0        0        0      685 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/managers/env.py
+-rw-r--r--   0        0        0     3116 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/managers/message.py
+-rw-r--r--   0        0        0     4526 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/managers/repo.py
+-rw-r--r--   0        0        0      800 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/managers/yaml.py
+-rw-r--r--   0        0        0        0 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/py.typed
+-rw-r--r--   0        0        0     2151 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/repo.py
+-rw-r--r--   0        0        0      759 2024-04-26 20:43:34.039297 pre_commit_update-0.3.1/src/pre_commit_update/utils.py
+-rw-r--r--   0        0        0     8158 1970-01-01 00:00:00.000000 pre_commit_update-0.3.1/PKG-INFO
```

### Comparing `pre_commit_update-0.3.0/LICENSE` & `pre_commit_update-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.0/README.md` & `pre_commit_update-0.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 <div align="center"><h1>pre-commit-update</h1>
 
 ![PyPI - Version](https://img.shields.io/pypi/v/pre-commit-update)
 ![PePy - Downloads](https://pepy.tech/badge/pre-commit-update)
-![Gitlab Pipeline Status](https://img.shields.io/gitlab/pipeline-status/vojko.pribudic%2Fpre-commit-update?branch=main&label=pipeline)
-![GitLab Issues](https://img.shields.io/gitlab/issues/open/vojko.pribudic%2Fpre-commit-update)
-![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/vojko.pribudic%2Fpre-commit-update)
-![GitLab Stars](https://img.shields.io/gitlab/stars/vojko.pribudic%2Fpre-commit-update?style=flat&color=%23FFD700)
+![Gitlab Pipeline Status](https://img.shields.io/gitlab/pipeline-status/vojko.pribudic.foss%2Fpre-commit-update?branch=main&label=pipeline)
+![GitLab Issues](https://img.shields.io/gitlab/issues/open/vojko.pribudic.foss%2Fpre-commit-update)
+![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/vojko.pribudic.foss%2Fpre-commit-update)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pre-commit-update)
 ![Python - Formatter](https://img.shields.io/badge/code%20style-black-black)
 ![PyPI - License](https://img.shields.io/pypi/l/pre-commit-update?color=%23333333)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pre-commit-update)
-![Codacy grade](https://img.shields.io/codacy/grade/7a7b10cc0e1e4197b838cdbcdb613bc8?logo=codacy)
+![Codacy grade](https://img.shields.io/codacy/grade/e727532ea95341b18ffd963e77605c2b?logo=codacy)
 </div>
 <div align="center">
 <a href="https://ko-fi.com/H2H8WN45E" target="_blank"><img alt="kofi" src="https://i.imgur.com/wdSRlJB.png" width="141" height="36"></a>
 
 <strong>pre-commit-update</strong> is a simple CLI tool to check and update pre-commit hooks.
 </div>
 
@@ -115,16 +114,16 @@
 **NOTE:** This is just an example, feel free to do your own configuration
 
 ### 2) pre-commit hook usage example
 
 You can also use `pre-commit-update` as a hook in your `pre-commit` hooks:
 
 ```yaml
-- repo: https://gitlab.com/vojko.pribudic/pre-commit-update
-  rev: v0.3.0  # Insert the latest tag here
+- repo: https://gitlab.com/vojko.pribudic.foss/pre-commit-update
+  rev: v0.3.1  # Insert the latest tag here
   hooks:
     - id: pre-commit-update
       args: [--dry-run, --exclude, black, --keep, isort]
 ```
 
 ### 3) pyproject.toml usage example
```

#### html2text {}

```diff
@@ -1,22 +1,21 @@
                         ************ pprree--ccoommmmiitt--uuppddaattee ************
   ![PyPI - Version](https://img.shields.io/pypi/v/pre-commit-update) ![PePy -
 Downloads](https://pepy.tech/badge/pre-commit-update) ![Gitlab Pipeline Status]
-  (https://img.shields.io/gitlab/pipeline-status/vojko.pribudic%2Fpre-commit-
-  update?branch=main&label=pipeline) ![GitLab Issues](https://img.shields.io/
- gitlab/issues/open/vojko.pribudic%2Fpre-commit-update) ![GitLab Last Commit]
-(https://img.shields.io/gitlab/last-commit/vojko.pribudic%2Fpre-commit-update)
-   ![GitLab Stars](https://img.shields.io/gitlab/stars/vojko.pribudic%2Fpre-
-commit-update?style=flat&color=%23FFD700) ![Libraries.io dependency status for
+   (https://img.shields.io/gitlab/pipeline-status/vojko.pribudic.foss%2Fpre-
+      commit-update?branch=main&label=pipeline) ![GitLab Issues](https://
+ img.shields.io/gitlab/issues/open/vojko.pribudic.foss%2Fpre-commit-update) !
+        [GitLab Last Commit](https://img.shields.io/gitlab/last-commit/
+ vojko.pribudic.foss%2Fpre-commit-update) ![Libraries.io dependency status for
   latest release](https://img.shields.io/librariesio/release/pypi/pre-commit-
 update) ![Python - Formatter](https://img.shields.io/badge/code%20style-black-
       black) ![PyPI - License](https://img.shields.io/pypi/l/pre-commit-
  update?color=%23333333) ![PyPI - Python Version](https://img.shields.io/pypi/
  pyversions/pre-commit-update) ![Codacy grade](https://img.shields.io/codacy/
-              grade/7a7b10cc0e1e4197b838cdbcdb613bc8?logo=codacy)
+              grade/e727532ea95341b18ffd963e77605c2b?logo=codacy)
   _[_k_o_f_i_]pprree--ccoommmmiitt--uuppddaattee is a simple CLI tool to check and update pre-commit
                                     hooks.
 ## Table of contents 1. [ Reasoning ](#1-reasoning) 2. [ Features ](#2-
 features) 3. [ Installation ](#3-installation) 4. [ Usage ](#4-usage) 1.
 [ Pipeline usage example ](#1-pipeline-usage-example) 1. [ GitLab job ](#a-
 gitlab-job) 2. [ pre-commit hook usage example ](#2-pre-commit-hook-usage-
 example) 3. [ pyproject.toml usage example ](#3-pyprojecttoml-usage-example) ##
@@ -55,23 +54,24 @@
 trim: https://github.com/ambv/black -> `black` (you will only pass `black` as a
 parameter to `exclude` or `keep`) ### 1) Pipeline usage example #### a) GitLab
 job: ```yaml pre-commit-hooks-update: stage: update script: # install git if
 not present in the image - pip install pre-commit-update - pre-commit-update --
 dry-run except: - main when: manual allow_failure: true ``` **NOTE:** This is
 just an example, feel free to do your own configuration ### 2) pre-commit hook
 usage example You can also use `pre-commit-update` as a hook in your `pre-
-commit` hooks: ```yaml - repo: https://gitlab.com/vojko.pribudic/pre-commit-
-update rev: v0.3.0 # Insert the latest tag here hooks: - id: pre-commit-update
-args: [--dry-run, --exclude, black, --keep, isort] ``` ### 3) pyproject.toml
-usage example You can configure `pre-commit-update` in your `pyproject.toml` as
-below (feel free to do your own configuration): ```toml [tool.pre-commit-
-update] dry_run = true all_versions = false verbose = true exclude = ["isort"]
-keep = ["black"] ``` **NOTE:** If some of the options are missing (for example
-`exclude` option), `pre-commit-update` will use default value for that option
-(default for `exclude` option would be an empty list). ***IMPORTANT*** If you
-invoke `pre-commit-update` with any arguments (e.g. `pre-commit-update -d`),
-`pyproject.toml` configuration will be **overridden**. This means that all the
-arguments passed while calling `pre-commit-update` will have priority over
-configuration defined inside `pyproject.toml`. If you want to override boolean
-flags, you can do so by passing the negative flag value. For example, given the
-configuration above, to override `verbose` flag from `pyproject.toml`, you
-would invoke `pre-commit-update` with either `--no-verbose` or `-nv`.
+commit` hooks: ```yaml - repo: https://gitlab.com/vojko.pribudic.foss/pre-
+commit-update rev: v0.3.1 # Insert the latest tag here hooks: - id: pre-commit-
+update args: [--dry-run, --exclude, black, --keep, isort] ``` ### 3)
+pyproject.toml usage example You can configure `pre-commit-update` in your
+`pyproject.toml` as below (feel free to do your own configuration): ```toml
+[tool.pre-commit-update] dry_run = true all_versions = false verbose = true
+exclude = ["isort"] keep = ["black"] ``` **NOTE:** If some of the options are
+missing (for example `exclude` option), `pre-commit-update` will use default
+value for that option (default for `exclude` option would be an empty list).
+***IMPORTANT*** If you invoke `pre-commit-update` with any arguments (e.g.
+`pre-commit-update -d`), `pyproject.toml` configuration will be **overridden**.
+This means that all the arguments passed while calling `pre-commit-update` will
+have priority over configuration defined inside `pyproject.toml`. If you want
+to override boolean flags, you can do so by passing the negative flag value.
+For example, given the configuration above, to override `verbose` flag from
+`pyproject.toml`, you would invoke `pre-commit-update` with either `--no-
+verbose` or `-nv`.
```

### Comparing `pre_commit_update-0.3.0/pyproject.toml` & `pre_commit_update-0.3.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [tool.poetry]
 name = "pre-commit-update"
-version = "0.3.0"
+version = "0.3.1"
 description = "Simple CLI tool to check and update pre-commit hooks."
 authors = ["Vojko Pribudić <dmanthing@gmail.com>"]
 maintainers = ["Vojko Pribudić <dmanthing@gmail.com>"]
-repository = "https://gitlab.com/vojko.pribudic/pre-commit-update"
+repository = "https://gitlab.com/vojko.pribudic.foss/pre-commit-update"
 readme = "README.md"
 license = "MIT"
 classifiers = [
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
@@ -27,16 +27,16 @@
 include = ["README.md", "LICENSE"]
 exclude = [
     ".gitignore",
     ".gitlab-ci.yml",
 ]
 
 [tool.poetry.urls]
-"Tracker" = "https://gitlab.com/vojko.pribudic/pre-commit-update/-/issues"
-"Changelog" = "https://gitlab.com/vojko.pribudic/pre-commit-update/-/releases"
+"Tracker" = "https://gitlab.com/vojko.pribudic.foss/pre-commit-update/-/issues"
+"Changelog" = "https://gitlab.com/vojko.pribudic.foss/pre-commit-update/-/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 click = ">=8.1"
 GitPython = ">=3.1"
 packaging = ">=23.2"
 pyproject-parser = ">=0.9"
```

### Comparing `pre_commit_update-0.3.0/src/pre_commit_update/cli.py` & `pre_commit_update-0.3.1/src/pre_commit_update/cli.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.0/src/pre_commit_update/managers/env.py` & `pre_commit_update-0.3.1/src/pre_commit_update/managers/env.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.0/src/pre_commit_update/managers/message.py` & `pre_commit_update-0.3.1/src/pre_commit_update/managers/message.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.0/src/pre_commit_update/managers/repo.py` & `pre_commit_update-0.3.1/src/pre_commit_update/managers/repo.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.0/src/pre_commit_update/managers/yaml.py` & `pre_commit_update-0.3.1/src/pre_commit_update/managers/yaml.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.0/src/pre_commit_update/repo.py` & `pre_commit_update-0.3.1/src/pre_commit_update/repo.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.0/src/pre_commit_update/utils.py` & `pre_commit_update-0.3.1/src/pre_commit_update/utils.py`

 * *Files identical despite different names*

### Comparing `pre_commit_update-0.3.0/PKG-INFO` & `pre_commit_update-0.3.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: pre-commit-update
-Version: 0.3.0
+Version: 0.3.1
 Summary: Simple CLI tool to check and update pre-commit hooks.
-Home-page: https://gitlab.com/vojko.pribudic/pre-commit-update
+Home-page: https://gitlab.com/vojko.pribudic.foss/pre-commit-update
 License: MIT
 Author: Vojko Pribudić
 Author-email: dmanthing@gmail.com
 Maintainer: Vojko Pribudić
 Maintainer-email: dmanthing@gmail.com
 Requires-Python: >=3.8
 Classifier: Development Status :: 5 - Production/Stable
@@ -25,32 +25,31 @@
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: GitPython (>=3.1)
 Requires-Dist: click (>=8.1)
 Requires-Dist: packaging (>=23.2)
 Requires-Dist: pyproject-parser (>=0.9)
 Requires-Dist: ruamel.yaml (>=0.18)
-Project-URL: Changelog, https://gitlab.com/vojko.pribudic/pre-commit-update/-/releases
-Project-URL: Repository, https://gitlab.com/vojko.pribudic/pre-commit-update
-Project-URL: Tracker, https://gitlab.com/vojko.pribudic/pre-commit-update/-/issues
+Project-URL: Changelog, https://gitlab.com/vojko.pribudic.foss/pre-commit-update/-/releases
+Project-URL: Repository, https://gitlab.com/vojko.pribudic.foss/pre-commit-update
+Project-URL: Tracker, https://gitlab.com/vojko.pribudic.foss/pre-commit-update/-/issues
 Description-Content-Type: text/markdown
 
 <div align="center"><h1>pre-commit-update</h1>
 
 ![PyPI - Version](https://img.shields.io/pypi/v/pre-commit-update)
 ![PePy - Downloads](https://pepy.tech/badge/pre-commit-update)
-![Gitlab Pipeline Status](https://img.shields.io/gitlab/pipeline-status/vojko.pribudic%2Fpre-commit-update?branch=main&label=pipeline)
-![GitLab Issues](https://img.shields.io/gitlab/issues/open/vojko.pribudic%2Fpre-commit-update)
-![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/vojko.pribudic%2Fpre-commit-update)
-![GitLab Stars](https://img.shields.io/gitlab/stars/vojko.pribudic%2Fpre-commit-update?style=flat&color=%23FFD700)
+![Gitlab Pipeline Status](https://img.shields.io/gitlab/pipeline-status/vojko.pribudic.foss%2Fpre-commit-update?branch=main&label=pipeline)
+![GitLab Issues](https://img.shields.io/gitlab/issues/open/vojko.pribudic.foss%2Fpre-commit-update)
+![GitLab Last Commit](https://img.shields.io/gitlab/last-commit/vojko.pribudic.foss%2Fpre-commit-update)
 ![Libraries.io dependency status for latest release](https://img.shields.io/librariesio/release/pypi/pre-commit-update)
 ![Python - Formatter](https://img.shields.io/badge/code%20style-black-black)
 ![PyPI - License](https://img.shields.io/pypi/l/pre-commit-update?color=%23333333)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/pre-commit-update)
-![Codacy grade](https://img.shields.io/codacy/grade/7a7b10cc0e1e4197b838cdbcdb613bc8?logo=codacy)
+![Codacy grade](https://img.shields.io/codacy/grade/e727532ea95341b18ffd963e77605c2b?logo=codacy)
 </div>
 <div align="center">
 <a href="https://ko-fi.com/H2H8WN45E" target="_blank"><img alt="kofi" src="https://i.imgur.com/wdSRlJB.png" width="141" height="36"></a>
 
 <strong>pre-commit-update</strong> is a simple CLI tool to check and update pre-commit hooks.
 </div>
 
@@ -151,16 +150,16 @@
 **NOTE:** This is just an example, feel free to do your own configuration
 
 ### 2) pre-commit hook usage example
 
 You can also use `pre-commit-update` as a hook in your `pre-commit` hooks:
 
 ```yaml
-- repo: https://gitlab.com/vojko.pribudic/pre-commit-update
-  rev: v0.3.0  # Insert the latest tag here
+- repo: https://gitlab.com/vojko.pribudic.foss/pre-commit-update
+  rev: v0.3.1  # Insert the latest tag here
   hooks:
     - id: pre-commit-update
       args: [--dry-run, --exclude, black, --keep, isort]
 ```
 
 ### 3) pyproject.toml usage example
```

#### html2text {}

```diff
@@ -1,43 +1,42 @@
-Metadata-Version: 2.1 Name: pre-commit-update Version: 0.3.0 Summary: Simple
+Metadata-Version: 2.1 Name: pre-commit-update Version: 0.3.1 Summary: Simple
 CLI tool to check and update pre-commit hooks. Home-page: https://gitlab.com/
-vojko.pribudic/pre-commit-update License: MIT Author: Vojko PribudiÄ Author-
-email: dmanthing@gmail.com Maintainer: Vojko PribudiÄ Maintainer-email:
+vojko.pribudic.foss/pre-commit-update License: MIT Author: Vojko PribudiÄ
+Author-email: dmanthing@gmail.com Maintainer: Vojko PribudiÄ Maintainer-email:
 dmanthing@gmail.com Requires-Python: >=3.8 Classifier: Development Status :: 5
 - Production/Stable Classifier: Environment :: Web Environment Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Natural Language :: English Classifier: Operating System ::
 OS Independent Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
 Programming Language :: Python :: 3 :: Only Classifier: Topic :: Software
 Development :: Libraries Requires-Dist: GitPython (>=3.1) Requires-Dist: click
 (>=8.1) Requires-Dist: packaging (>=23.2) Requires-Dist: pyproject-parser
 (>=0.9) Requires-Dist: ruamel.yaml (>=0.18) Project-URL: Changelog, https://
-gitlab.com/vojko.pribudic/pre-commit-update/-/releases Project-URL: Repository,
-https://gitlab.com/vojko.pribudic/pre-commit-update Project-URL: Tracker,
-https://gitlab.com/vojko.pribudic/pre-commit-update/-/issues Description-
-Content-Type: text/markdown
+gitlab.com/vojko.pribudic.foss/pre-commit-update/-/releases Project-URL:
+Repository, https://gitlab.com/vojko.pribudic.foss/pre-commit-update Project-
+URL: Tracker, https://gitlab.com/vojko.pribudic.foss/pre-commit-update/-/issues
+Description-Content-Type: text/markdown
                         ************ pprree--ccoommmmiitt--uuppddaattee ************
   ![PyPI - Version](https://img.shields.io/pypi/v/pre-commit-update) ![PePy -
 Downloads](https://pepy.tech/badge/pre-commit-update) ![Gitlab Pipeline Status]
-  (https://img.shields.io/gitlab/pipeline-status/vojko.pribudic%2Fpre-commit-
-  update?branch=main&label=pipeline) ![GitLab Issues](https://img.shields.io/
- gitlab/issues/open/vojko.pribudic%2Fpre-commit-update) ![GitLab Last Commit]
-(https://img.shields.io/gitlab/last-commit/vojko.pribudic%2Fpre-commit-update)
-   ![GitLab Stars](https://img.shields.io/gitlab/stars/vojko.pribudic%2Fpre-
-commit-update?style=flat&color=%23FFD700) ![Libraries.io dependency status for
+   (https://img.shields.io/gitlab/pipeline-status/vojko.pribudic.foss%2Fpre-
+      commit-update?branch=main&label=pipeline) ![GitLab Issues](https://
+ img.shields.io/gitlab/issues/open/vojko.pribudic.foss%2Fpre-commit-update) !
+        [GitLab Last Commit](https://img.shields.io/gitlab/last-commit/
+ vojko.pribudic.foss%2Fpre-commit-update) ![Libraries.io dependency status for
   latest release](https://img.shields.io/librariesio/release/pypi/pre-commit-
 update) ![Python - Formatter](https://img.shields.io/badge/code%20style-black-
       black) ![PyPI - License](https://img.shields.io/pypi/l/pre-commit-
  update?color=%23333333) ![PyPI - Python Version](https://img.shields.io/pypi/
  pyversions/pre-commit-update) ![Codacy grade](https://img.shields.io/codacy/
-              grade/7a7b10cc0e1e4197b838cdbcdb613bc8?logo=codacy)
+              grade/e727532ea95341b18ffd963e77605c2b?logo=codacy)
   _[_k_o_f_i_]pprree--ccoommmmiitt--uuppddaattee is a simple CLI tool to check and update pre-commit
                                     hooks.
 ## Table of contents 1. [ Reasoning ](#1-reasoning) 2. [ Features ](#2-
 features) 3. [ Installation ](#3-installation) 4. [ Usage ](#4-usage) 1.
 [ Pipeline usage example ](#1-pipeline-usage-example) 1. [ GitLab job ](#a-
 gitlab-job) 2. [ pre-commit hook usage example ](#2-pre-commit-hook-usage-
 example) 3. [ pyproject.toml usage example ](#3-pyprojecttoml-usage-example) ##
@@ -76,23 +75,24 @@
 trim: https://github.com/ambv/black -> `black` (you will only pass `black` as a
 parameter to `exclude` or `keep`) ### 1) Pipeline usage example #### a) GitLab
 job: ```yaml pre-commit-hooks-update: stage: update script: # install git if
 not present in the image - pip install pre-commit-update - pre-commit-update --
 dry-run except: - main when: manual allow_failure: true ``` **NOTE:** This is
 just an example, feel free to do your own configuration ### 2) pre-commit hook
 usage example You can also use `pre-commit-update` as a hook in your `pre-
-commit` hooks: ```yaml - repo: https://gitlab.com/vojko.pribudic/pre-commit-
-update rev: v0.3.0 # Insert the latest tag here hooks: - id: pre-commit-update
-args: [--dry-run, --exclude, black, --keep, isort] ``` ### 3) pyproject.toml
-usage example You can configure `pre-commit-update` in your `pyproject.toml` as
-below (feel free to do your own configuration): ```toml [tool.pre-commit-
-update] dry_run = true all_versions = false verbose = true exclude = ["isort"]
-keep = ["black"] ``` **NOTE:** If some of the options are missing (for example
-`exclude` option), `pre-commit-update` will use default value for that option
-(default for `exclude` option would be an empty list). ***IMPORTANT*** If you
-invoke `pre-commit-update` with any arguments (e.g. `pre-commit-update -d`),
-`pyproject.toml` configuration will be **overridden**. This means that all the
-arguments passed while calling `pre-commit-update` will have priority over
-configuration defined inside `pyproject.toml`. If you want to override boolean
-flags, you can do so by passing the negative flag value. For example, given the
-configuration above, to override `verbose` flag from `pyproject.toml`, you
-would invoke `pre-commit-update` with either `--no-verbose` or `-nv`.
+commit` hooks: ```yaml - repo: https://gitlab.com/vojko.pribudic.foss/pre-
+commit-update rev: v0.3.1 # Insert the latest tag here hooks: - id: pre-commit-
+update args: [--dry-run, --exclude, black, --keep, isort] ``` ### 3)
+pyproject.toml usage example You can configure `pre-commit-update` in your
+`pyproject.toml` as below (feel free to do your own configuration): ```toml
+[tool.pre-commit-update] dry_run = true all_versions = false verbose = true
+exclude = ["isort"] keep = ["black"] ``` **NOTE:** If some of the options are
+missing (for example `exclude` option), `pre-commit-update` will use default
+value for that option (default for `exclude` option would be an empty list).
+***IMPORTANT*** If you invoke `pre-commit-update` with any arguments (e.g.
+`pre-commit-update -d`), `pyproject.toml` configuration will be **overridden**.
+This means that all the arguments passed while calling `pre-commit-update` will
+have priority over configuration defined inside `pyproject.toml`. If you want
+to override boolean flags, you can do so by passing the negative flag value.
+For example, given the configuration above, to override `verbose` flag from
+`pyproject.toml`, you would invoke `pre-commit-update` with either `--no-
+verbose` or `-nv`.
```

