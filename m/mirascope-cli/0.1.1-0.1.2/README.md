# Comparing `tmp/mirascope_cli-0.1.1.tar.gz` & `tmp/mirascope_cli-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mirascope_cli-0.1.1.tar", max compression
+gzip compressed data, was "mirascope_cli-0.1.2.tar", max compression
```

## Comparing `mirascope_cli-0.1.1.tar` & `mirascope_cli-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1066 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/LICENSE
--rw-r--r--   0        0        0     7516 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/docs/README.md
--rw-r--r--   0        0        0       98 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/__init__.py
--rw-r--r--   0        0        0      199 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/commands/__init__.py
--rw-r--r--   0        0        0     4212 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/commands/add.py
--rw-r--r--   0        0        0     3002 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/commands/init.py
--rw-r--r--   0        0        0        0 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/commands/py.typed
--rw-r--r--   0        0        0     3101 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/commands/remove.py
--rw-r--r--   0        0        0     2008 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/commands/status.py
--rw-r--r--   0        0        0     2800 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/commands/use.py
--rw-r--r--   0        0        0      118 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/constants.py
--rw-r--r--   0        0        0      980 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/enums.py
--rw-r--r--   0        0        0       86 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/generic/__init__.py
--rw-r--r--   0        0        0      494 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/generic/mirascope.ini.j2
--rw-r--r--   0        0        0     1556 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/generic/prompt_template.j2
--rw-r--r--   0        0        0     1067 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/main.py
--rw-r--r--   0        0        0        0 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/py.typed
--rw-r--r--   0        0        0     1582 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/schemas.py
--rw-r--r--   0        0        0    26969 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/mirascope_cli/utils.py
--rw-r--r--   0        0        0     1803 2024-04-17 01:31:05.354824 mirascope_cli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8307 1970-01-01 00:00:00.000000 mirascope_cli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7529 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/docs/README.md
+-rw-r--r--   0        0        0       98 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/__init__.py
+-rw-r--r--   0        0        0      199 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/__init__.py
+-rw-r--r--   0        0        0     4212 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/add.py
+-rw-r--r--   0        0        0     3002 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/init.py
+-rw-r--r--   0        0        0        0 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/py.typed
+-rw-r--r--   0        0        0     3101 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/remove.py
+-rw-r--r--   0        0        0     2008 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/status.py
+-rw-r--r--   0        0        0     2800 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/commands/use.py
+-rw-r--r--   0        0        0      118 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/constants.py
+-rw-r--r--   0        0        0      980 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/enums.py
+-rw-r--r--   0        0        0       86 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/generic/__init__.py
+-rw-r--r--   0        0        0      494 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/generic/mirascope.ini.j2
+-rw-r--r--   0        0        0     1556 2024-04-26 19:06:18.914903 mirascope_cli-0.1.2/mirascope_cli/generic/prompt_template.j2
+-rw-r--r--   0        0        0     1067 2024-04-26 19:06:18.918902 mirascope_cli-0.1.2/mirascope_cli/main.py
+-rw-r--r--   0        0        0        0 2024-04-26 19:06:18.918902 mirascope_cli-0.1.2/mirascope_cli/py.typed
+-rw-r--r--   0        0        0     1582 2024-04-26 19:06:18.918902 mirascope_cli-0.1.2/mirascope_cli/schemas.py
+-rw-r--r--   0        0        0    26969 2024-04-26 19:06:18.918902 mirascope_cli-0.1.2/mirascope_cli/utils.py
+-rw-r--r--   0        0        0     1804 2024-04-26 19:06:18.918902 mirascope_cli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8319 1970-01-01 00:00:00.000000 mirascope_cli-0.1.2/PKG-INFO
```

### Comparing `mirascope_cli-0.1.1/LICENSE` & `mirascope_cli-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.1/docs/README.md` & `mirascope_cli-0.1.2/docs/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -165,17 +165,16 @@
 
 ```shell
 mirascope remove book_recommender 0001
 ```
 
 Here you specify which prompt and version you want to remove. Removal will delete the file but also update any versions that have the deleted version in their `prev_revision_id` to `None`.
 
-!!! note
-
-    `mirascope remove` will not remove the prompt if `current_revision` is the same as the prompt you are trying to remove. You can use `mirascope add` if you have incoming changes or `mirascope use` to swap `current_revision`.
+> [!NOTE]
+> `mirascope remove` will not remove the prompt if `current_revision` is the same as the prompt you are trying to remove. You can use `mirascope add` if you have incoming changes or `mirascope use` to swap `current_revision`.
 
 ## Mirascope INI
 
 The Mirascope INI provides some customization for you. Feel free to update any field.
 
 ```python
 [mirascope]
@@ -202,12 +201,12 @@
 
 - `auto_tag` - Adds `@tags(["version:0001"])` to Mirascope Prompts. This will auto increment the version number if a new version is added.
 
 ## Future updates
 
 There is a lot more to be added to the Mirascope CLI. Here is a list in no order of things we are thinking about adding next:
 
-- prompt comparison - A way to compare two different versions with a golden test
-- history - View the revision history of a version
-- testing - Adding input and outputs to the revision for CI testing
+- [ ]  prompt comparison - A way to compare two different versions with a golden test
+- [ ]  history - View the revision history of a version
+- [ ]  testing - Adding input and outputs to the revision for CI testing
 
 If you want some of these features implemented or if you think something is useful but not on this list, let us know!
```

### Comparing `mirascope_cli-0.1.1/mirascope_cli/commands/add.py` & `mirascope_cli-0.1.2/mirascope_cli/commands/add.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.1/mirascope_cli/commands/init.py` & `mirascope_cli-0.1.2/mirascope_cli/commands/init.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.1/mirascope_cli/commands/remove.py` & `mirascope_cli-0.1.2/mirascope_cli/commands/remove.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.1/mirascope_cli/commands/status.py` & `mirascope_cli-0.1.2/mirascope_cli/commands/status.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.1/mirascope_cli/commands/use.py` & `mirascope_cli-0.1.2/mirascope_cli/commands/use.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.1/mirascope_cli/enums.py` & `mirascope_cli-0.1.2/mirascope_cli/enums.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.1/mirascope_cli/generic/prompt_template.j2` & `mirascope_cli-0.1.2/mirascope_cli/generic/prompt_template.j2`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.1/mirascope_cli/main.py` & `mirascope_cli-0.1.2/mirascope_cli/main.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.1/mirascope_cli/schemas.py` & `mirascope_cli-0.1.2/mirascope_cli/schemas.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.1/mirascope_cli/utils.py` & `mirascope_cli-0.1.2/mirascope_cli/utils.py`

 * *Files identical despite different names*

### Comparing `mirascope_cli-0.1.1/pyproject.toml` & `mirascope_cli-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "mirascope-cli"
-version = "0.1.1"
+version = "0.1.2"
 description = "The Mirascope Command Line Interface"
 license = "MIT"
 authors = [
     "William Bakst <william@mirascope.io>",
     "Brendan Kao <brendan@mirascope.io>",
 ]
 readme = "docs/README.md"
 packages = [{ include = "mirascope_cli" }]
 repository = "https://github.com/Mirascope/mirascope-cli"
 
 [tool.poetry.scripts]
 mirascope = 'mirascope_cli.main:app'
 
 [tool.poetry.dependencies]
-python = ">=3.9,<3.13"
+python = ">=3.9,<4.0"
 pydantic = "^2.0.2"
 typer = { version = ">=0.9.0,<1.0.0", extras = ["all"] }
 Jinja2 = "^3.1.3"
 
 [tool.poetry.group.dev.dependencies]
-mirascope = ">=0.9.1,<1.0.0"
+# mirascope = ">=0.9.1,<1.0.0"
 mypy = "^1.6.1"
 pytest = "^7.4.0"
 ruff = "^0.1.5"
 pytest-asyncio = "^0.23.3"
 pytest-cov = "^4.1.0"
 
 [tool.poetry.group.docs.dependencies]
```

### Comparing `mirascope_cli-0.1.1/PKG-INFO` & `mirascope_cli-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: mirascope-cli
-Version: 0.1.1
+Version: 0.1.2
 Summary: The Mirascope Command Line Interface
 Home-page: https://github.com/Mirascope/mirascope-cli
 License: MIT
 Author: William Bakst
 Author-email: william@mirascope.io
-Requires-Python: >=3.9,<3.13
+Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: Jinja2 (>=3.1.3,<4.0.0)
@@ -186,17 +186,16 @@
 
 ```shell
 mirascope remove book_recommender 0001
 ```
 
 Here you specify which prompt and version you want to remove. Removal will delete the file but also update any versions that have the deleted version in their `prev_revision_id` to `None`.
 
-!!! note
-
-    `mirascope remove` will not remove the prompt if `current_revision` is the same as the prompt you are trying to remove. You can use `mirascope add` if you have incoming changes or `mirascope use` to swap `current_revision`.
+> [!NOTE]
+> `mirascope remove` will not remove the prompt if `current_revision` is the same as the prompt you are trying to remove. You can use `mirascope add` if you have incoming changes or `mirascope use` to swap `current_revision`.
 
 ## Mirascope INI
 
 The Mirascope INI provides some customization for you. Feel free to update any field.
 
 ```python
 [mirascope]
@@ -223,13 +222,13 @@
 
 - `auto_tag` - Adds `@tags(["version:0001"])` to Mirascope Prompts. This will auto increment the version number if a new version is added.
 
 ## Future updates
 
 There is a lot more to be added to the Mirascope CLI. Here is a list in no order of things we are thinking about adding next:
 
-- prompt comparison - A way to compare two different versions with a golden test
-- history - View the revision history of a version
-- testing - Adding input and outputs to the revision for CI testing
+- [ ]  prompt comparison - A way to compare two different versions with a golden test
+- [ ]  history - View the revision history of a version
+- [ ]  testing - Adding input and outputs to the revision for CI testing
 
 If you want some of these features implemented or if you think something is useful but not on this list, let us know!
```

