# Comparing `tmp/uodm-0.1.2.tar.gz` & `tmp/uodm-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uodm-0.1.2.tar", last modified: Wed Apr 24 16:35:58 2024, max compression
+gzip compressed data, was "uodm-0.1.3.tar", last modified: Fri Apr 26 10:09:45 2024, max compression
```

## Comparing `uodm-0.1.2.tar` & `uodm-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1211 2024-04-23 12:08:19.992618 uodm-0.1.2/LICENSE
--rw-r--r--   0        0        0     2451 2024-04-23 13:49:15.123787 uodm-0.1.2/README.md
--rw-r--r--   0        0        0      488 2024-04-24 16:35:58.014645 uodm-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      667 2024-04-23 12:55:06.946411 uodm-0.1.2/src/uodm/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 15:22:51.793479 uodm-0.1.2/src/uodm/py.typed
--rw-r--r--   0        0        0     6085 2024-04-24 16:35:40.277939 uodm-0.1.2/src/uodm/uodm.py
--rw-r--r--   0        0        0        0 2024-04-23 12:45:59.201089 uodm-0.1.2/tests/__init__.py
--rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 uodm-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-23 12:08:19.992618 uodm-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2451 2024-04-23 13:49:15.123787 uodm-0.1.3/README.md
+-rw-r--r--   0        0        0      488 2024-04-26 10:09:45.856880 uodm-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      667 2024-04-23 12:55:06.946411 uodm-0.1.3/src/uodm/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 15:22:51.793479 uodm-0.1.3/src/uodm/py.typed
+-rw-r--r--   0        0        0     6249 2024-04-26 10:08:27.508515 uodm-0.1.3/src/uodm/uodm.py
+-rw-r--r--   0        0        0        0 2024-04-23 12:45:59.201089 uodm-0.1.3/tests/__init__.py
+-rw-r--r--   0        0        0     2794 1970-01-01 00:00:00.000000 uodm-0.1.3/PKG-INFO
```

### Comparing `uodm-0.1.2/LICENSE` & `uodm-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uodm-0.1.2/README.md` & `uodm-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `uodm-0.1.2/src/uodm/__init__.py` & `uodm-0.1.3/src/uodm/__init__.py`

 * *Files identical despite different names*

### Comparing `uodm-0.1.2/src/uodm/uodm.py` & `uodm-0.1.3/src/uodm/uodm.py`

 * *Files 2% similar despite different names*

```diff
@@ -118,14 +118,19 @@
         dmp = self.model_dump()
         if not self.model_validate(dmp):
             raise ValueError("Model validation failed")
         await collection.update_one(
             {"_id": self._id}, {"$set": self.model_dump()}, upsert=True
         )
 
+    async def delete(self):
+        collection = self.get_collection()
+        if self._id is not None:
+            await collection.delete_one({"_id": self._id})
+
     @classmethod
     def get_model_config(cls: Type[T]) -> dict:
         res = {}
         if conf_coll := getattr(cls, "__collection__", None):
             res["collection"] = conf_coll
         if conf_indexes := getattr(cls, "__indexes__", None):
             res["indexes"] = conf_indexes
```

### Comparing `uodm-0.1.2/PKG-INFO` & `uodm-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uodm
-Version: 0.1.2
+Version: 0.1.3
 Summary: ultraminimalistic Python library for simple object-document mappint for asyncronous mongodb
 Author-Email: Grigory Bakunov <bobuk@rubedo.cloud>
 License: Unlicense
 Requires-Python: >=3.12
 Requires-Dist: pydantic>=2.7.0
 Requires-Dist: motor>=3.4.0
 Description-Content-Type: text/markdown
```

