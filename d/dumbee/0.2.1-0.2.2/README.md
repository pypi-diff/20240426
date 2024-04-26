# Comparing `tmp/dumbee-0.2.1.tar.gz` & `tmp/dumbee-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dumbee-0.2.1.tar", last modified: Fri Mar  8 19:55:45 2024, max compression
+gzip compressed data, was "dumbee-0.2.2.tar", last modified: Fri Apr 26 19:57:26 2024, max compression
```

## Comparing `dumbee-0.2.1.tar` & `dumbee-0.2.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:45.839008 dumbee-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-08 19:55:45.839008 dumbee-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-08 19:55:39.000000 dumbee-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:45.835008 dumbee-0.2.1/dumbee/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:45.835008 dumbee-0.2.1/dumbee/core/
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/core/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/core/engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/core/middlewaring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/core/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/core/query.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:45.835008 dumbee-0.2.1/dumbee/drivers/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/drivers/filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:45.835008 dumbee-0.2.1/dumbee/ext/
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/ext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:45.835008 dumbee-0.2.1/dumbee/ext/json/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/ext/json/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/ext/json/serialization.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:45.835008 dumbee-0.2.1/dumbee/ext/jsonschema/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/ext/jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/ext/jsonschema/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:45.835008 dumbee-0.2.1/dumbee/ext/logging/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/ext/logging/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:45.835008 dumbee-0.2.1/dumbee/ext/pydantic/
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/ext/pydantic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-08 19:55:39.000000 dumbee-0.2.1/dumbee/ext/pydantic/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:45.839008 dumbee-0.2.1/dumbee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-08 19:55:45.000000 dumbee-0.2.1/dumbee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-03-08 19:55:45.000000 dumbee-0.2.1/dumbee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-08 19:55:45.000000 dumbee-0.2.1/dumbee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-08 19:55:45.000000 dumbee-0.2.1/dumbee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-08 19:55:45.000000 dumbee-0.2.1/dumbee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-08 19:55:45.839008 dumbee-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      702 2024-03-08 19:55:39.000000 dumbee-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:45.839008 dumbee-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-08 19:55:39.000000 dumbee-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-03-08 19:55:39.000000 dumbee-0.2.1/tests/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:26.365555 dumbee-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-26 19:57:26.365555 dumbee-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-26 19:57:22.000000 dumbee-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:26.361555 dumbee-0.2.2/dumbee/
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:26.365555 dumbee-0.2.2/dumbee/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/core/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/core/engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/core/middlewaring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4543 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/core/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/core/query.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:26.365555 dumbee-0.2.2/dumbee/drivers/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/drivers/filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:26.365555 dumbee-0.2.2/dumbee/ext/
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/ext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:26.365555 dumbee-0.2.2/dumbee/ext/json/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/ext/json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1494 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/ext/json/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:26.365555 dumbee-0.2.2/dumbee/ext/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/ext/jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1978 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/ext/jsonschema/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:26.365555 dumbee-0.2.2/dumbee/ext/logging/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/ext/logging/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:26.365555 dumbee-0.2.2/dumbee/ext/pydantic/
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/ext/pydantic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-26 19:57:22.000000 dumbee-0.2.2/dumbee/ext/pydantic/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:26.365555 dumbee-0.2.2/dumbee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-04-26 19:57:26.000000 dumbee-0.2.2/dumbee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-04-26 19:57:26.000000 dumbee-0.2.2/dumbee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-26 19:57:26.000000 dumbee-0.2.2/dumbee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-26 19:57:26.000000 dumbee-0.2.2/dumbee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-26 19:57:26.000000 dumbee-0.2.2/dumbee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-26 19:57:26.365555 dumbee-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      702 2024-04-26 19:57:22.000000 dumbee-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:26.365555 dumbee-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-26 19:57:22.000000 dumbee-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-26 19:57:22.000000 dumbee-0.2.2/tests/main.py
```

### Comparing `dumbee-0.2.1/PKG-INFO` & `dumbee-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumbee
-Version: 0.2.1
+Version: 0.2.2
 Summary: A dumb database, not for production
 Home-page: https://github.com/dschenck/dumbee
 Author: David Schenck
 Author-email: david.schenck@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dumbee-0.2.1/README.md` & `dumbee-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `dumbee-0.2.1/dumbee/core/driver.py` & `dumbee-0.2.2/dumbee/core/driver.py`

 * *Files identical despite different names*

### Comparing `dumbee-0.2.1/dumbee/core/engine.py` & `dumbee-0.2.2/dumbee/core/engine.py`

 * *Files identical despite different names*

### Comparing `dumbee-0.2.1/dumbee/core/middlewaring.py` & `dumbee-0.2.2/dumbee/core/middlewaring.py`

 * *Files identical despite different names*

### Comparing `dumbee-0.2.1/dumbee/core/nodes.py` & `dumbee-0.2.2/dumbee/core/nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,14 +123,25 @@
 
 
 class Collection(Node):
     """
     Collection of documents
     """
 
+    def __contains__(self, name: str) -> bool:
+        """
+        Returns True if a record of the given name exists
+        in this collection
+
+        Returns
+        -------
+        bool
+        """
+        return self.get(name).exists()
+
     def insert(self, id=None) -> Record:
         """
         Returns a Record
 
         Returns
         -------
         Record
@@ -182,14 +193,21 @@
 
     def __getitem__(self, name) -> Collection:
         """
         Get a collection by name
         """
         return Collection(f"{self.path}/{name}", self.engine)
 
+    def __contains__(self, name: str) -> bool:
+        """
+        Returns True if a collection of the given name
+        exists in the collections
+        """
+        return self[name].exists()
+
     def all(self) -> typing.List[Collection]:
         """
         Returns all the collections under the current node
 
         Returns
         -------
         list[Collection]
```

### Comparing `dumbee-0.2.1/dumbee/core/query.py` & `dumbee-0.2.2/dumbee/core/query.py`

 * *Files identical despite different names*

### Comparing `dumbee-0.2.1/dumbee/drivers/filesystem.py` & `dumbee-0.2.2/dumbee/drivers/filesystem.py`

 * *Files identical despite different names*

### Comparing `dumbee-0.2.1/dumbee/ext/json/serialization.py` & `dumbee-0.2.2/dumbee/ext/json/serialization.py`

 * *Files identical despite different names*

### Comparing `dumbee-0.2.1/dumbee/ext/jsonschema/validation.py` & `dumbee-0.2.2/dumbee/ext/jsonschema/validation.py`

 * *Files identical despite different names*

### Comparing `dumbee-0.2.1/dumbee.egg-info/PKG-INFO` & `dumbee-0.2.2/dumbee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dumbee
-Version: 0.2.1
+Version: 0.2.2
 Summary: A dumb database, not for production
 Home-page: https://github.com/dschenck/dumbee
 Author: David Schenck
 Author-email: david.schenck@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `dumbee-0.2.1/dumbee.egg-info/SOURCES.txt` & `dumbee-0.2.2/dumbee.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dumbee-0.2.1/setup.py` & `dumbee-0.2.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="dumbee",
-    version="0.2.1",
+    version="0.2.2",
     author="David Schenck",
     author_email="david.schenck@outlook.com",
     description="A dumb database, not for production",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dschenck/dumbee",
     packages=setuptools.find_packages(),
```

### Comparing `dumbee-0.2.1/tests/main.py` & `dumbee-0.2.2/tests/main.py`

 * *Files identical despite different names*

