# Comparing `tmp/pulp-cli-gem-0.4.0.tar.gz` & `tmp/pulp-cli-gem-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-cli-gem-0.4.0.tar", last modified: Mon Mar 18 12:05:02 2024, max compression
+gzip compressed data, was "pulp-cli-gem-0.5.0.tar", last modified: Fri Apr 26 10:30:50 2024, max compression
```

## Comparing `pulp-cli-gem-0.4.0.tar` & `pulp-cli-gem-0.5.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:05:02.478340 pulp-cli-gem-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-18 12:05:02.478340 pulp-cli-gem-0.4.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:05:02.478340 pulp-cli-gem-0.4.0/pulp_cli_gem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      808 2024-03-18 12:05:02.000000 pulp-cli-gem-0.4.0/pulp_cli_gem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-18 12:05:02.000000 pulp-cli-gem-0.4.0/pulp_cli_gem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 12:05:02.000000 pulp-cli-gem-0.4.0/pulp_cli_gem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-18 12:05:02.000000 pulp-cli-gem-0.4.0/pulp_cli_gem.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-03-18 12:05:02.000000 pulp-cli-gem-0.4.0/pulp_cli_gem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-03-18 12:05:02.000000 pulp-cli-gem-0.4.0/pulp_cli_gem.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:05:02.474340 pulp-cli-gem-0.4.0/pulpcore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:05:02.474340 pulp-cli-gem-0.4.0/pulpcore/cli/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:05:02.478340 pulp-cli-gem-0.4.0/pulpcore/cli/gem/
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-03-18 12:04:51.000000 pulp-cli-gem-0.4.0/pulpcore/cli/gem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-03-18 12:04:51.000000 pulp-cli-gem-0.4.0/pulpcore/cli/gem/content.py
--rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-03-18 12:04:51.000000 pulp-cli-gem-0.4.0/pulpcore/cli/gem/distribution.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-18 12:04:51.000000 pulp-cli-gem-0.4.0/pulpcore/cli/gem/publication.py
--rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-03-18 12:04:51.000000 pulp-cli-gem-0.4.0/pulpcore/cli/gem/remote.py
--rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-03-18 12:04:51.000000 pulp-cli-gem-0.4.0/pulpcore/cli/gem/repository.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-03-18 12:04:51.000000 pulp-cli-gem-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 12:05:02.478340 pulp-cli-gem-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:30:50.489668 pulp-cli-gem-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-26 10:30:50.489668 pulp-cli-gem-0.5.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:30:50.485668 pulp-cli-gem-0.5.0/pulp_cli_gem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-26 10:30:50.000000 pulp-cli-gem-0.5.0/pulp_cli_gem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-26 10:30:50.000000 pulp-cli-gem-0.5.0/pulp_cli_gem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:30:50.000000 pulp-cli-gem-0.5.0/pulp_cli_gem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-26 10:30:50.000000 pulp-cli-gem-0.5.0/pulp_cli_gem.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-26 10:30:50.000000 pulp-cli-gem-0.5.0/pulp_cli_gem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-26 10:30:50.000000 pulp-cli-gem-0.5.0/pulp_cli_gem.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:30:50.485668 pulp-cli-gem-0.5.0/pulpcore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:30:50.485668 pulp-cli-gem-0.5.0/pulpcore/cli/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:30:50.489668 pulp-cli-gem-0.5.0/pulpcore/cli/gem/
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-26 10:30:44.000000 pulp-cli-gem-0.5.0/pulpcore/cli/gem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3886 2024-04-26 10:30:44.000000 pulp-cli-gem-0.5.0/pulpcore/cli/gem/content.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2819 2024-04-26 10:30:44.000000 pulp-cli-gem-0.5.0/pulpcore/cli/gem/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-26 10:30:44.000000 pulp-cli-gem-0.5.0/pulpcore/cli/gem/publication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2259 2024-04-26 10:30:44.000000 pulp-cli-gem-0.5.0/pulpcore/cli/gem/remote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4890 2024-04-26 10:30:44.000000 pulp-cli-gem-0.5.0/pulpcore/cli/gem/repository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4108 2024-04-26 10:30:44.000000 pulp-cli-gem-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:30:50.489668 pulp-cli-gem-0.5.0/setup.cfg
```

### Comparing `pulp-cli-gem-0.4.0/PKG-INFO` & `pulp-cli-gem-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-cli-gem
-Version: 0.4.0
+Version: 0.5.0
 Summary: Command line interface to talk to pulpcore's REST API. (Gem plugin commands)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-gem
 Project-URL: changelog, https://github.com/pulp/pulp-cli-gem/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pulp-cli-gem-0.4.0/pulp_cli_gem.egg-info/PKG-INFO` & `pulp-cli-gem-0.5.0/pulp_cli_gem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-cli-gem
-Version: 0.4.0
+Version: 0.5.0
 Summary: Command line interface to talk to pulpcore's REST API. (Gem plugin commands)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-gem
 Project-URL: changelog, https://github.com/pulp/pulp-cli-gem/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

### Comparing `pulp-cli-gem-0.4.0/pulpcore/cli/gem/__init__.py` & `pulp-cli-gem-0.5.0/pulpcore/cli/gem/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pulpcore.cli.gem.publication import publication
 from pulpcore.cli.gem.remote import remote
 from pulpcore.cli.gem.repository import repository
 
 translation = get_translation(__package__)
 _ = translation.gettext
 
-__version__ = "0.4.0"
+__version__ = "0.5.0"
 
 
 @pulp_group(name="gem")
 def gem_group() -> None:
     pass
```

### Comparing `pulp-cli-gem-0.4.0/pulpcore/cli/gem/content.py` & `pulp-cli-gem-0.5.0/pulpcore/cli/gem/content.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-gem-0.4.0/pulpcore/cli/gem/distribution.py` & `pulp-cli-gem-0.5.0/pulpcore/cli/gem/distribution.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-gem-0.4.0/pulpcore/cli/gem/publication.py` & `pulp-cli-gem-0.5.0/pulpcore/cli/gem/publication.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-gem-0.4.0/pulpcore/cli/gem/remote.py` & `pulp-cli-gem-0.5.0/pulpcore/cli/gem/remote.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-gem-0.4.0/pulpcore/cli/gem/repository.py` & `pulp-cli-gem-0.5.0/pulpcore/cli/gem/repository.py`

 * *Files identical despite different names*

### Comparing `pulp-cli-gem-0.4.0/pyproject.toml` & `pulp-cli-gem-0.5.0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pulp-cli-gem"
-version = "0.4.0"
+version = "0.5.0"
 description = "Command line interface to talk to pulpcore's REST API. (Gem plugin commands)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "GPLv2+"}
 authors = [
   {name = "Pulp Team", email = "pulp-list@redhat.com"},
 ]
@@ -19,16 +19,16 @@
   "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Topic :: System :: Software Distribution",
   "Typing :: Typed",
 ]
 dependencies = [
-  "pulp-cli>=0.23.1,<0.25",
-  "pulp-glue-gem==0.4.0",
+  "pulp-cli>=0.23.1,<0.26",
+  "pulp-glue-gem==0.5.0",
 ]
 
 [project.urls]
 repository = "https://github.com/pulp/pulp-cli-gem"
 changelog = "https://github.com/pulp/pulp-cli-gem/blob/main/CHANGES.md"
 
 [project.entry-points."pulp_cli.plugins"]
@@ -39,26 +39,21 @@
 include = ["pulpcore.cli.*"]
 namespaces = true
 
 [tool.setuptools.package-data]
 "*" = ["py.typed", "locale/*/LC_MESSAGES/*.mo"]
 
 [tool.pulp_cli_template]
+# This section is co-managed by the cookiecutter templates.
+# Changes to existing keys should be preserved.
 app_label = "gem"
 glue = true
 docs = false
 translations = false
-test_matrix = """
-- python: "3.11"
-  image_tag: "nightly"
-  pulp_api_root: "/relocated/djnd/"
-- python: "3.8"
-  image_tag: "latest"
-  lower_bounds: true
-"""
+main_package = "gem"
 
 [tool.towncrier]
 filename = "CHANGES.md"
 directory = "CHANGES/"
 title_format = "## {version} ({project_date})"
 template = "CHANGES/.TEMPLATE.md"
 issue_format = "[#{issue}](https://github.com/pulp/pulp-cli-gem/issues/{issue})"
@@ -131,7 +126,50 @@
 
 [[tool.mypy.overrides]]
 module = [
   "click_shell.*",
   "schema.*",
 ]
 ignore_missing_imports = true
+
+[tool.bumpversion]
+# This section is managed by the cookiecutter templates.
+current_version = "0.5.0"
+commit = false
+tag = false
+parse = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)(\\.(?P<release>[a-z]+))?"
+serialize = [
+  "{major}.{minor}.{patch}.{release}",
+  "{major}.{minor}.{patch}",
+]
+
+[tool.bumpversion.parts.release]
+optional_value = "prod"
+values = [
+  "dev",
+  "prod",
+]
+
+[[tool.bumpversion.files]]
+filename = "./pulp-glue-gem/pulp_glue/gem/__init__.py"
+search = "__version__ = \"{current_version}\""
+replace = "__version__ = \"{new_version}\""
+
+[[tool.bumpversion.files]]
+filename = "./pulpcore/cli/gem/__init__.py"
+search = "__version__ = \"{current_version}\""
+replace = "__version__ = \"{new_version}\""
+
+[[tool.bumpversion.files]]
+filename = "./pulp-glue-gem/pyproject.toml"
+search = "version = \"{current_version}\""
+replace = "version = \"{new_version}\""
+
+[[tool.bumpversion.files]]
+filename = "./pyproject.toml"
+search = "version = \"{current_version}\""
+replace = "version = \"{new_version}\""
+
+[[tool.bumpversion.files]]
+filename = "./pyproject.toml"
+search = "\"pulp-glue-gem=={current_version}\""
+replace = "\"pulp-glue-gem=={new_version}\""
```

