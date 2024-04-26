# Comparing `tmp/pulp-glue-gem-0.4.0.tar.gz` & `tmp/pulp-glue-gem-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulp-glue-gem-0.4.0.tar", last modified: Mon Mar 18 12:05:01 2024, max compression
+gzip compressed data, was "pulp-glue-gem-0.5.0.tar", last modified: Fri Apr 26 10:30:49 2024, max compression
```

## Comparing `pulp-glue-gem-0.4.0.tar` & `pulp-glue-gem-0.5.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:05:01.302340 pulp-glue-gem-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-18 12:05:01.302340 pulp-glue-gem-0.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 12:04:51.000000 pulp-glue-gem-0.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:05:01.302340 pulp-glue-gem-0.4.0/pulp_glue/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:05:01.302340 pulp-glue-gem-0.4.0/pulp_glue/gem/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 12:04:51.000000 pulp-glue-gem-0.4.0/pulp_glue/gem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3120 2024-03-18 12:04:51.000000 pulp-glue-gem-0.4.0/pulp_glue/gem/context.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-18 12:04:51.000000 pulp-glue-gem-0.4.0/pulp_glue/gem/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-18 12:05:01.302340 pulp-glue-gem-0.4.0/pulp_glue_gem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-03-18 12:05:01.000000 pulp-glue-gem-0.4.0/pulp_glue_gem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-03-18 12:05:01.000000 pulp-glue-gem-0.4.0/pulp_glue_gem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-18 12:05:01.000000 pulp-glue-gem-0.4.0/pulp_glue_gem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-03-18 12:05:01.000000 pulp-glue-gem-0.4.0/pulp_glue_gem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-18 12:05:01.000000 pulp-glue-gem-0.4.0/pulp_glue_gem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-03-18 12:04:51.000000 pulp-glue-gem-0.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-18 12:05:01.302340 pulp-glue-gem-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:30:49.337659 pulp-glue-gem-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-26 10:30:49.337659 pulp-glue-gem-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:30:44.000000 pulp-glue-gem-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:30:49.333659 pulp-glue-gem-0.5.0/pulp_glue/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:30:49.333659 pulp-glue-gem-0.5.0/pulp_glue/gem/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-26 10:30:44.000000 pulp-glue-gem-0.5.0/pulp_glue/gem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 2024-04-26 10:30:44.000000 pulp-glue-gem-0.5.0/pulp_glue/gem/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 10:30:44.000000 pulp-glue-gem-0.5.0/pulp_glue/gem/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 10:30:49.337659 pulp-glue-gem-0.5.0/pulp_glue_gem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-26 10:30:49.000000 pulp-glue-gem-0.5.0/pulp_glue_gem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-26 10:30:49.000000 pulp-glue-gem-0.5.0/pulp_glue_gem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 10:30:49.000000 pulp-glue-gem-0.5.0/pulp_glue_gem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-26 10:30:49.000000 pulp-glue-gem-0.5.0/pulp_glue_gem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-26 10:30:49.000000 pulp-glue-gem-0.5.0/pulp_glue_gem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-26 10:30:44.000000 pulp-glue-gem-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 10:30:49.337659 pulp-glue-gem-0.5.0/setup.cfg
```

### Comparing `pulp-glue-gem-0.4.0/PKG-INFO` & `pulp-glue-gem-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue-gem
-Version: 0.4.0
+Version: 0.5.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API. (Gem plugin)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-gem
 Project-URL: changelog, https://github.com/pulp/pulp-cli-gem/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-gem-0.4.0/pulp_glue/gem/context.py` & `pulp-glue-gem-0.5.0/pulp_glue/gem/context.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     ENTITY = _("gem distribution")
     ENTITIES = _("gem distributions")
     HREF = "gem_gem_distribution_href"
     ID_PREFIX = "distributions_gem_gem"
     NEEDS_PLUGINS = [PluginRequirement("gem")]
     CAPABILITIES = {"roles": [PluginRequirement("gem", specifier=">=0.4.0.dev")]}
 
-    def preprocess_body(self, body: EntityDefinition) -> EntityDefinition:
-        body = super().preprocess_body(body)
+    def preprocess_entity(self, body: EntityDefinition, partial: bool = False) -> EntityDefinition:
+        body = super().preprocess_entity(body)
         version = body.pop("version", None)
         if version is not None:
             repository_href = body.pop("repository")
             body["repository_version"] = f"{repository_href}versions/{version}/"
         return body
```

### Comparing `pulp-glue-gem-0.4.0/pulp_glue_gem.egg-info/PKG-INFO` & `pulp-glue-gem-0.5.0/pulp_glue_gem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulp-glue-gem
-Version: 0.4.0
+Version: 0.5.0
 Summary: Version agnostic glue library to talk to pulpcore's REST API. (Gem plugin)
 Author-email: Pulp Team <pulp-list@redhat.com>
 License: GPLv2+
 Project-URL: repository, https://github.com/pulp/pulp-cli-gem
 Project-URL: changelog, https://github.com/pulp/pulp-cli-gem/blob/main/CHANGES.md
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

### Comparing `pulp-glue-gem-0.4.0/pyproject.toml` & `pulp-glue-gem-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pulp-glue-gem"
-version = "0.4.0"
+version = "0.5.0"
 description = "Version agnostic glue library to talk to pulpcore's REST API. (Gem plugin)"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {text = "GPLv2+"}
 authors = [
   {name = "Pulp Team", email = "pulp-list@redhat.com"},
 ]
@@ -19,15 +19,15 @@
   "License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)",
   "Operating System :: OS Independent",
   "Programming Language :: Python :: 3",
   "Topic :: System :: Software Distribution",
   "Typing :: Typed",
 ]
 dependencies = [
-  "pulp-glue>=0.23.1,<0.25.0",
+  "pulp-glue>=0.23.1,<0.26",
 ]
 
 [project.urls]
 repository = "https://github.com/pulp/pulp-cli-gem"
 changelog = "https://github.com/pulp/pulp-cli-gem/blob/main/CHANGES.md"
 
 [tool.setuptools.packages.find]
```

