# Comparing `tmp/stinky_noodle-0.0.5.tar.gz` & `tmp/stinky_noodle-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stinky_noodle-0.0.5.tar", last modified: Fri Apr 26 20:21:21 2024, max compression
+gzip compressed data, was "stinky_noodle-0.0.7.tar", last modified: Fri Apr 26 20:36:15 2024, max compression
```

## Comparing `stinky_noodle-0.0.5.tar` & `stinky_noodle-0.0.7.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:21.885215 stinky_noodle-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-26 20:21:21.885215 stinky_noodle-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:21:21.885215 stinky_noodle-0.0.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:21.881215 stinky_noodle-0.0.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:21.881215 stinky_noodle-0.0.5/src/stinky/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/src/stinky/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:21.881215 stinky_noodle-0.0.5/src/stinky/noodle/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/src/stinky/noodle/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/src/stinky/noodle/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:21.885215 stinky_noodle-0.0.5/src/stinky/noodle/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/src/stinky/noodle/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/src/stinky/noodle/utils/builtins.py
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/src/stinky/noodle/utils/enforcer.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/src/stinky/noodle/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/src/stinky/noodle/utils/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/src/stinky/noodle/utils/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-26 20:21:17.000000 stinky_noodle-0.0.5/src/stinky/noodle/utils/ruleset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:21:21.885215 stinky_noodle-0.0.5/src/stinky_noodle.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-26 20:21:21.000000 stinky_noodle-0.0.5/src/stinky_noodle.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-26 20:21:21.000000 stinky_noodle-0.0.5/src/stinky_noodle.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:21:21.000000 stinky_noodle-0.0.5/src/stinky_noodle.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 20:21:21.000000 stinky_noodle-0.0.5/src/stinky_noodle.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 20:21:21.000000 stinky_noodle-0.0.5/src/stinky_noodle.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 20:21:21.000000 stinky_noodle-0.0.5/src/stinky_noodle.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:15.525505 stinky_noodle-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-26 20:36:15.525505 stinky_noodle-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 20:36:15.525505 stinky_noodle-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:15.521505 stinky_noodle-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:15.521505 stinky_noodle-0.0.7/src/stinky/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/src/stinky/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:15.521505 stinky_noodle-0.0.7/src/stinky/noodle/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/src/stinky/noodle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/src/stinky/noodle/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:15.521505 stinky_noodle-0.0.7/src/stinky/noodle/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/src/stinky/noodle/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/src/stinky/noodle/utils/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/src/stinky/noodle/utils/enforcer.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/src/stinky/noodle/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/src/stinky/noodle/utils/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/src/stinky/noodle/utils/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-26 20:36:11.000000 stinky_noodle-0.0.7/src/stinky/noodle/utils/ruleset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 20:36:15.525505 stinky_noodle-0.0.7/src/stinky_noodle.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-26 20:36:15.000000 stinky_noodle-0.0.7/src/stinky_noodle.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-26 20:36:15.000000 stinky_noodle-0.0.7/src/stinky_noodle.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 20:36:15.000000 stinky_noodle-0.0.7/src/stinky_noodle.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 20:36:15.000000 stinky_noodle-0.0.7/src/stinky_noodle.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-26 20:36:15.000000 stinky_noodle-0.0.7/src/stinky_noodle.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-26 20:36:15.000000 stinky_noodle-0.0.7/src/stinky_noodle.egg-info/top_level.txt
```

### Comparing `stinky_noodle-0.0.5/PKG-INFO` & `stinky_noodle-0.0.7/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stinky-noodle
-Version: 0.0.5
+Version: 0.0.7
 Summary: Stinky noodle is a Python-based OpenAPI spec linter compatible with spectral rulesets
 Author-email: Riccardo Tiebax <riccardo.t@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pyjsonpath==1.2.3
 Provides-Extra: tests
```

### Comparing `stinky_noodle-0.0.5/README.md` & `stinky_noodle-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `stinky_noodle-0.0.5/pyproject.toml` & `stinky_noodle-0.0.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "stinky-noodle"
-version = "0.0.5"
+version = "0.0.7"
 description = "Stinky noodle is a Python-based OpenAPI spec linter compatible with spectral rulesets"
 authors = [
     { name = "Riccardo Tiebax", email = "riccardo.t@gmail.com" },
 ]
 readme = "README.md"
 dependencies = [
     "loguru==0.7.2",
@@ -36,19 +36,19 @@
 
 [tool.isort]
 profile = "black"
 known_third_party = ["pytest"]
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.0.5"
+version = "0.0.7"
 tag_format = "$version"
 changelog_incremental = true
 update_changelog_on_bump = true
 version_files = ["src/stinky/__init__.py:__version__", "pyproject.toml:^version"]
-bump_message = "release $current_version -> $new_version ***NO_CI***"
+bump_message = "release $current_version -> $new_version"
 
 [tool.deptry]
 ignore_notebooks = true
 
 [tool.deptry.per_rule_ignores]
 DEP001 = ["stinky"]
```

### Comparing `stinky_noodle-0.0.5/src/stinky/noodle/core.py` & `stinky_noodle-0.0.7/src/stinky/noodle/core.py`

 * *Files identical despite different names*

### Comparing `stinky_noodle-0.0.5/src/stinky/noodle/utils/builtins.py` & `stinky_noodle-0.0.7/src/stinky/noodle/utils/builtins.py`

 * *Files identical despite different names*

### Comparing `stinky_noodle-0.0.5/src/stinky/noodle/utils/enforcer.py` & `stinky_noodle-0.0.7/src/stinky/noodle/utils/enforcer.py`

 * *Files identical despite different names*

### Comparing `stinky_noodle-0.0.5/src/stinky/noodle/utils/ruleset.py` & `stinky_noodle-0.0.7/src/stinky/noodle/utils/ruleset.py`

 * *Files identical despite different names*

### Comparing `stinky_noodle-0.0.5/src/stinky_noodle.egg-info/PKG-INFO` & `stinky_noodle-0.0.7/src/stinky_noodle.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stinky-noodle
-Version: 0.0.5
+Version: 0.0.7
 Summary: Stinky noodle is a Python-based OpenAPI spec linter compatible with spectral rulesets
 Author-email: Riccardo Tiebax <riccardo.t@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: loguru==0.7.2
 Requires-Dist: pydantic==2.6.4
 Requires-Dist: pyjsonpath==1.2.3
 Provides-Extra: tests
```

### Comparing `stinky_noodle-0.0.5/src/stinky_noodle.egg-info/SOURCES.txt` & `stinky_noodle-0.0.7/src/stinky_noodle.egg-info/SOURCES.txt`

 * *Files identical despite different names*

