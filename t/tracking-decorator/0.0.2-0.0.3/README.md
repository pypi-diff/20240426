# Comparing `tmp/tracking_decorator-0.0.2.tar.gz` & `tmp/tracking_decorator-0.0.3.tar.gz`

## Comparing `tracking_decorator-0.0.2.tar` & `tracking_decorator-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 tracking_decorator-0.0.2/CHANGELOG.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tracking_decorator-0.0.2/src/tracking_decorator/__init__.py
--rw-r--r--   0        0        0     1788 2020-02-02 00:00:00.000000 tracking_decorator-0.0.2/src/tracking_decorator/track_changes.py
--rw-r--r--   0        0        0     1951 2020-02-02 00:00:00.000000 tracking_decorator-0.0.2/tests/test_track_changes.py
--rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 tracking_decorator-0.0.2/.gitignore
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tracking_decorator-0.0.2/LICENSE
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 tracking_decorator-0.0.2/README.md
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 tracking_decorator-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 tracking_decorator-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/CHANGELOG.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/src/tracking_decorator/__init__.py
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/src/tracking_decorator/track_changes.py
+-rw-r--r--   0        0        0     1898 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/src/tracking_decorator/trash_collections.py
+-rw-r--r--   0        0        0     2910 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/tests/test_track_changes.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/LICENSE
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/README.md
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 tracking_decorator-0.0.3/PKG-INFO
```

### Comparing `tracking_decorator-0.0.2/.gitignore` & `tracking_decorator-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `tracking_decorator-0.0.2/LICENSE` & `tracking_decorator-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tracking_decorator-0.0.2/README.md` & `tracking_decorator-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `tracking_decorator-0.0.2/pyproject.toml` & `tracking_decorator-0.0.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
+[tool.pytest.ini_options]
+pythonpath = ["src"]
+testpaths = ["tests"]
+
 [project]
 name = "tracking_decorator"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ian Lavine", email="ian.lavine@mail.utoronto.ca" },
 ]
 description = "A small decorator for tracking changed attributes in a class"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `tracking_decorator-0.0.2/PKG-INFO` & `tracking_decorator-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: tracking_decorator
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small decorator for tracking changed attributes in a class
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Issues, https://github.com/pypa/sampleproject/issues
 Author-email: Ian Lavine <ian.lavine@mail.utoronto.ca>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

