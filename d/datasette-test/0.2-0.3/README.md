# Comparing `tmp/datasette-test-0.2.tar.gz` & `tmp/datasette_test-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datasette-test-0.2.tar", last modified: Tue Jan 16 22:36:22 2024, max compression
+gzip compressed data, was "datasette_test-0.3.tar", last modified: Fri Apr 26 18:23:55 2024, max compression
```

## Comparing `datasette-test-0.2.tar` & `datasette_test-0.3.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 22:36:22.439059 datasette-test-0.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-01-16 22:36:11.000000 datasette-test-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-01-16 22:36:22.439059 datasette-test-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-01-16 22:36:11.000000 datasette-test-0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 22:36:22.439059 datasette-test-0.2/datasette_test/
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2024-01-16 22:36:11.000000 datasette-test-0.2/datasette_test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 22:36:22.439059 datasette-test-0.2/datasette_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3250 2024-01-16 22:36:22.000000 datasette-test-0.2/datasette_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-01-16 22:36:22.000000 datasette-test-0.2/datasette_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 22:36:22.000000 datasette-test-0.2/datasette_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-01-16 22:36:22.000000 datasette-test-0.2/datasette_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-01-16 22:36:22.000000 datasette-test-0.2/datasette_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-01-16 22:36:11.000000 datasette-test-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 22:36:22.439059 datasette-test-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 22:36:22.439059 datasette-test-0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-01-16 22:36:11.000000 datasette-test-0.2/tests/test_datasette_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:23:55.302247 datasette_test-0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-26 18:23:46.000000 datasette_test-0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-26 18:23:55.302247 datasette_test-0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-26 18:23:46.000000 datasette_test-0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:23:55.298247 datasette_test-0.3/datasette_test/
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-26 18:23:46.000000 datasette_test-0.3/datasette_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      433 2024-04-26 18:23:46.000000 datasette_test-0.3/datasette_test/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:23:55.298247 datasette_test-0.3/datasette_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-26 18:23:55.000000 datasette_test-0.3/datasette_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      792 2024-04-26 18:23:46.000000 datasette_test-0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 18:23:55.302247 datasette_test-0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 18:23:55.298247 datasette_test-0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-26 18:23:46.000000 datasette_test-0.3/tests/test_datasette_test.py
```

### Comparing `datasette-test-0.2/LICENSE` & `datasette_test-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datasette-test-0.2/PKG-INFO` & `datasette_test-0.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,7 @@
-Metadata-Version: 2.1
-Name: datasette-test
-Version: 0.2
-Summary: Utilities to help write tests for Datasette plugins and applications
-Author: Datasette
-License: Apache-2.0
-Project-URL: Homepage, https://github.com/datasette/datasette-test
-Project-URL: Changelog, https://github.com/datasette/datasette-test/releases
-Project-URL: Issues, https://github.com/datasette/datasette-test/issues
-Project-URL: CI, https://github.com/datasette/datasette-test/actions
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: datasette
-Requires-Dist: httpx
-Provides-Extra: test
-Requires-Dist: pytest; extra == "test"
-Requires-Dist: pytest-asyncio; extra == "test"
-
 # datasette-test
 
 [![PyPI](https://img.shields.io/pypi/v/datasette-test.svg)](https://pypi.org/project/datasette-test/)
 [![Tests](https://github.com/datasette/datasette-test/actions/workflows/test.yml/badge.svg)](https://github.com/datasette/datasette-test/actions/workflows/test.yml)
 [![Changelog](https://img.shields.io/github/v/release/datasette/datasette-test?include_prereleases&label=changelog)](https://github.com/datasette/datasette-test/releases)
 [![License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://github.com/datasette/datasette-test/blob/main/LICENSE)
 
@@ -49,14 +29,26 @@
 async def test_datasette():
     ds = Datasette(plugin_config={"my-plugin": {"config": "goes here"})
 ```
 This subclass detects if the underlying plugin needs configuration in metadata or config and instantiates the class correctly either way.
 
 You can also use this class while continuing to pass `metadata={"plugins": ...}` - the class will move that configuration to config when necessary.
 
+## permissions= convenience argument
+
+Datasette 1.0a introduces a [more convenient way](https://docs.datasette.io/en/1.0a13/authentication.html#other-permissions-in-datasette-yaml) of defining permissions directly in the configuration:
+```python
+ds = Datasette(config={"permissions": {"view-instance": {"id": "root"}}})
+```
+This is not supported by Datasette pre 1.0 - but you can use the `permissions=` argument in `datasette_test.Datasette` to achieve the same effect:
+```python
+ds = Datasette(permissions={"view-instance": {"id": "root"}})
+```
+This will work across both major Datasette versions.
+
 ## wait_until_responds(url, timeout=5.0)
 
 Some Datasette plugin test suites launch a Datasette server and then need to wait for that server to become available before continuing.
 
 Call this function to wait until the server becomes available, or raise an error if it takes longer than the timeout:
 
 ```python
@@ -64,14 +56,30 @@
 
 def test_server():
     # ... start server ...
     wait_until_responds("http://localhost:8001")
     # Now run tests
 ```
 
+## actor_cookie(datasette, actor)
+
+Equivalent to `datasette.client.actor_cookie()` in Datasette 1.0a+. Example usage:
+
+```python
+@pytest.mark.asyncio
+async def test_permissions():
+    ds = Datasette(permissions={"view-instance": {"id": "root"}})
+    response = await ds.client.get("/")
+    assert response.status_code == 403
+    response = await ds.client.get(
+        "/", cookies={"ds_actor": actor_cookie(ds, {"id": "root"})}
+    )
+    assert response.status_code == 200
+```
+
 ## Development
 
 To contribute to this library, first checkout the code. Then create a new virtual environment:
 ```bash
 cd datasette-test
 python -m venv venv
 source venv/bin/activate
```

### Comparing `datasette-test-0.2/datasette_test/__init__.py` & `datasette_test-0.3/datasette_test/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 from datasette.app import Datasette as _Datasette
+from datasette.version import __version__
+from packaging.version import parse
 import time
 import httpx
 
 
-try:
-    from datasette.utils import fail_if_plugins_in_metadata
-
-    plugin_config_should_be_in_metadata = False
-except ImportError:
-    plugin_config_should_be_in_metadata = True
+plugin_config_should_be_in_metadata = parse(__version__) < parse("1.0a8")
 
 
 class Datasette(_Datasette):
     def __init__(self, *args, **kwargs):
         plugin_config = kwargs.pop("plugin_config", None)
         if plugin_config is not None:
             if plugin_config_should_be_in_metadata:
@@ -27,19 +24,36 @@
             "plugins" in (kwargs.get("metadata") or {})
             and not plugin_config_should_be_in_metadata
         ):
             # Move plugins to config anyway
             plugin_config = kwargs["metadata"].pop("plugins")
             kwargs["config"] = kwargs.get("config") or {}
             kwargs["config"]["plugins"] = plugin_config
+        permissions = kwargs.pop("permissions", None)
+        if permissions:
+            if plugin_config_should_be_in_metadata:
+                # Stash these to be handled by our special plugin
+                self._special_test_permissions = permissions
+            else:
+                # Put it in config
+                if "config" not in kwargs:
+                    kwargs["config"] = {}
+                kwargs["config"]["permissions"] = permissions
         super().__init__(*args, **kwargs)
 
 
 def wait_until_responds(url: str, timeout: float = 5.0):
     start = time.time()
     while time.time() - start < timeout:
         try:
             httpx.get(url)
             return
         except httpx.ConnectError:
             time.sleep(0.1)
     raise AssertionError("Timed out waiting for {} to respond".format(url))
+
+
+def actor_cookie(datasette, actor):
+    if hasattr(datasette.client, "actor_cookie"):
+        return datasette.client.actor_cookie({"id": "root"})
+    else:
+        return datasette.sign({"a": actor}, "actor")
```

### Comparing `datasette-test-0.2/pyproject.toml` & `datasette_test-0.3/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 [project]
 name = "datasette-test"
-version = "0.2"
+version = "0.3"
 description = "Utilities to help write tests for Datasette plugins and applications"
 readme = "README.md"
 requires-python = ">=3.8"
 authors = [{name = "Datasette"}]
 license = {text = "Apache-2.0"}
 classifiers = [
     "License :: OSI Approved :: Apache Software License"
 ]
 dependencies = [
     "datasette",
-    "httpx"
+    "httpx",
+    "packaging"
 ]
 
 [project.urls]
 Homepage = "https://github.com/datasette/datasette-test"
 Changelog = "https://github.com/datasette/datasette-test/releases"
 Issues = "https://github.com/datasette/datasette-test/issues"
 CI = "https://github.com/datasette/datasette-test/actions"
 
+[project.entry-points.datasette]
+datasette_test = "datasette_test.plugin"
+
 [project.optional-dependencies]
 test = ["pytest", "pytest-asyncio"]
```

