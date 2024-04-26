# Comparing `tmp/uodm-0.1.3.tar.gz` & `tmp/uodm-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uodm-0.1.3.tar", last modified: Fri Apr 26 10:09:45 2024, max compression
+gzip compressed data, was "uodm-0.1.4.tar", last modified: Fri Apr 26 10:40:25 2024, max compression
```

## Comparing `uodm-0.1.3.tar` & `uodm-0.1.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1211 2024-04-23 12:08:19.992618 uodm-0.1.3/LICENSE
--rw-r--r--   0        0        0     2451 2024-04-23 13:49:15.123787 uodm-0.1.3/README.md
--rw-r--r--   0        0        0      488 2024-04-26 10:09:45.856880 uodm-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      667 2024-04-23 12:55:06.946411 uodm-0.1.3/src/uodm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 15:22:51.793479 uodm-0.1.3/src/uodm/py.typed
--rw-r--r--   0        0        0     6249 2024-04-26 10:08:27.508515 uodm-0.1.3/src/uodm/uodm.py
--rw-r--r--   0        0        0        0 2024-04-23 12:45:59.201089 uodm-0.1.3/tests/__init__.py
--rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 uodm-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-23 12:08:19.992618 uodm-0.1.4/LICENSE
+-rw-r--r--   0        0        0     2451 2024-04-23 13:49:15.123787 uodm-0.1.4/README.md
+-rw-r--r--   0        0        0      488 2024-04-26 10:40:25.813713 uodm-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      667 2024-04-23 12:55:06.946411 uodm-0.1.4/src/uodm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 15:22:51.793479 uodm-0.1.4/src/uodm/py.typed
+-rw-r--r--   0        0        0     6493 2024-04-26 10:38:39.138408 uodm-0.1.4/src/uodm/uodm.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:45:59.201089 uodm-0.1.4/tests/__init__.py
+-rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 uodm-0.1.4/PKG-INFO
```

### Comparing `uodm-0.1.3/LICENSE` & `uodm-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `uodm-0.1.3/README.md` & `uodm-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `uodm-0.1.3/src/uodm/__init__.py` & `uodm-0.1.4/src/uodm/__init__.py`

 * *Files identical despite different names*

### Comparing `uodm-0.1.3/src/uodm/uodm.py` & `uodm-0.1.4/src/uodm/uodm.py`

 * *Files 8% similar despite different names*

```diff
@@ -192,8 +192,14 @@
     @staticmethod
     def filtering(**kwargs) -> dict:
         if "id" in kwargs:
             kwargs["_id"] = kwargs.pop("id")
         if "_id" in kwargs:
             if isinstance(kwargs["_id"], str):
                 kwargs["_id"] = ObjectId(kwargs["_id"])
+        args = kwargs.copy()
+        for arg in kwargs.keys():
+            if '_in_' in arg or '__' in arg:
+                key = arg.replace('_in_', '.').replace('__', '.')
+                args[key] = kwargs[arg]
+                del args[arg]
         return kwargs
```

### Comparing `uodm-0.1.3/PKG-INFO` & `uodm-0.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uodm
-Version: 0.1.3
+Version: 0.1.4
 Summary: ultraminimalistic Python library for simple object-document mappint for asyncronous mongodb
 Author-Email: Grigory Bakunov <bobuk@rubedo.cloud>
 License: Unlicense
 Requires-Python: >=3.12
 Requires-Dist: pydantic>=2.7.0
 Requires-Dist: motor>=3.4.0
 Description-Content-Type: text/markdown
```

