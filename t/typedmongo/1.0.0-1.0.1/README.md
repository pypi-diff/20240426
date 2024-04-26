# Comparing `tmp/typedmongo-1.0.0.tar.gz` & `tmp/typedmongo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-1.0.0.tar", last modified: Thu Apr 25 17:15:45 2024, max compression
+gzip compressed data, was "typedmongo-1.0.1.tar", last modified: Fri Apr 26 01:35:23 2024, max compression
```

## Comparing `typedmongo-1.0.0.tar` & `typedmongo-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-25 17:15:33.191543 typedmongo-1.0.0/LICENSE
--rw-r--r--   0        0        0      108 2024-04-25 17:15:33.191543 typedmongo-1.0.0/README.md
--rw-r--r--   0        0        0     1441 2024-04-25 17:15:45.719857 typedmongo-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/asyncio/__init__.py
--rw-r--r--   0        0        0     5347 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/asyncio/test_client.py
--rw-r--r--   0        0        0     2777 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/asyncio/test_table.py
--rw-r--r--   0        0        0     1218 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/sync.py
--rw-r--r--   0        0        0     5119 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/test_client.py
--rw-r--r--   0        0        0     2930 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/test_expressions.py
--rw-r--r--   0        0        0      582 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/test_marshamallow.py
--rw-r--r--   0        0        0     2769 2024-04-25 17:15:33.191543 typedmongo-1.0.0/tests/test_table.py
--rw-r--r--   0        0        0      749 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/__init__.py
--rw-r--r--   0        0        0      749 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    11778 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     8629 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     6954 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    11560 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5452 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/expressions.py
--rw-r--r--   0        0        0     8629 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/fields.py
--rw-r--r--   0        0        0      351 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/marshamallow.py
--rw-r--r--   0        0        0     1325 2024-04-25 17:15:33.191543 typedmongo-1.0.0/typedmongo/sync.py
--rw-r--r--   0        0        0     6948 2024-04-25 17:15:33.195543 typedmongo-1.0.0/typedmongo/table.py
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-26 01:35:09.653655 typedmongo-1.0.1/LICENSE
+-rw-r--r--   0        0        0      108 2024-04-26 01:35:09.653655 typedmongo-1.0.1/README.md
+-rw-r--r--   0        0        0     1441 2024-04-26 01:35:23.377765 typedmongo-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-26 01:35:09.653655 typedmongo-1.0.1/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 01:35:09.653655 typedmongo-1.0.1/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     5504 2024-04-26 01:35:09.653655 typedmongo-1.0.1/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     2620 2024-04-26 01:35:09.653655 typedmongo-1.0.1/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-04-26 01:35:09.653655 typedmongo-1.0.1/tests/sync.py
+-rw-r--r--   0        0        0     5276 2024-04-26 01:35:09.653655 typedmongo-1.0.1/tests/test_client.py
+-rw-r--r--   0        0        0     2930 2024-04-26 01:35:09.653655 typedmongo-1.0.1/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-04-26 01:35:09.653655 typedmongo-1.0.1/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     2612 2024-04-26 01:35:09.653655 typedmongo-1.0.1/tests/test_table.py
+-rw-r--r--   0        0        0      749 2024-04-26 01:35:09.653655 typedmongo-1.0.1/typedmongo/__init__.py
+-rw-r--r--   0        0        0      749 2024-04-26 01:35:09.653655 typedmongo-1.0.1/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    11778 2024-04-26 01:35:09.653655 typedmongo-1.0.1/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     8629 2024-04-26 01:35:09.653655 typedmongo-1.0.1/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     6982 2024-04-26 01:35:09.653655 typedmongo-1.0.1/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    11560 2024-04-26 01:35:09.657655 typedmongo-1.0.1/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-04-26 01:35:09.657655 typedmongo-1.0.1/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5452 2024-04-26 01:35:09.657655 typedmongo-1.0.1/typedmongo/expressions.py
+-rw-r--r--   0        0        0     8629 2024-04-26 01:35:09.657655 typedmongo-1.0.1/typedmongo/fields.py
+-rw-r--r--   0        0        0      351 2024-04-26 01:35:09.657655 typedmongo-1.0.1/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1325 2024-04-26 01:35:09.657655 typedmongo-1.0.1/typedmongo/sync.py
+-rw-r--r--   0        0        0     6982 2024-04-26 01:35:09.657655 typedmongo-1.0.1/typedmongo/table.py
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.0.1/PKG-INFO
```

### Comparing `typedmongo-1.0.0/LICENSE` & `typedmongo-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/pyproject.toml` & `typedmongo-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typedmongo"
-version = "1.0.0"
+version = "1.0.1"
 description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
```

### Comparing `typedmongo-1.0.0/tests/asyncio/test_client.py` & `typedmongo-1.0.1/tests/asyncio/test_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 class User(MongoTable):
     name: mongo.StringField
     age: mongo.IntegerField
     tags: mongo.ListField[str]
     wallet: mongo.EmbeddedField[Wallet]
     children: mongo.ListField[User]
 
+    @classmethod
+    def indexes(cls) -> list[mongo.Index]:
+        super_indexes = super().indexes()
+        return [*super_indexes, mongo.Index(cls.age)]
+
 
 # If use scope="module", the test will fail. Because pytest-asyncio close the event loop.
 @pytest.fixture(scope="function", autouse=True)
 async def init_models():
     await mongo.initial_collections(
         MongoClient().mongo,
         User,
```

### Comparing `typedmongo-1.0.0/tests/asyncio/test_table.py` & `typedmongo-1.0.1/tests/asyncio/test_table.py`

 * *Files 4% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 class User(MongoTable):
     name: mongo.StringField
     age: mongo.IntegerField
     tags: mongo.ListField[str]
     wallet: mongo.EmbeddedField[Wallet]
     children: mongo.ListField[User]
 
-    @classmethod
-    def indexes(cls) -> list[mongo.Index]:
-        super_indexes = super().indexes()
-        return [*super_indexes, mongo.Index(cls.age)]
-
 
 User.__lazy_init_fields__()
 
 
 @pytest.mark.parametrize(
     "expression, repr_str",
     [
```

### Comparing `typedmongo-1.0.0/tests/sync.py` & `typedmongo-1.0.1/tests/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/tests/test_client.py` & `typedmongo-1.0.1/tests/test_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,19 @@
 class User(MongoTable):
     name: mongo.StringField
     age: mongo.IntegerField
     tags: mongo.ListField[str]
     wallet: mongo.EmbeddedField[Wallet]
     children: mongo.ListField[User]
 
+    @classmethod
+    def indexes(cls) -> list[mongo.Index]:
+        super_indexes = super().indexes()
+        return [*super_indexes, mongo.Index(cls.age)]
+
 
 # If use scope="module", the test will fail. Because pytest-asyncio close the event loop.
 @pytest.fixture(scope="function", autouse=True)
 def init_models():
     mongo.initial_collections(
         MongoClient().mongo,
         User,
```

### Comparing `typedmongo-1.0.0/tests/test_expressions.py` & `typedmongo-1.0.1/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/tests/test_marshamallow.py` & `typedmongo-1.0.1/tests/test_marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/tests/test_table.py` & `typedmongo-1.0.1/tests/test_table.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,19 +21,14 @@
 class User(MongoTable):
     name: mongo.StringField
     age: mongo.IntegerField
     tags: mongo.ListField[str]
     wallet: mongo.EmbeddedField[Wallet]
     children: mongo.ListField[User]
 
-    @classmethod
-    def indexes(cls) -> list[mongo.Index]:
-        super_indexes = super().indexes()
-        return [*super_indexes, mongo.Index(cls.age)]
-
 
 User.__lazy_init_fields__()
 
 
 @pytest.mark.parametrize(
     "expression, repr_str",
     [
```

### Comparing `typedmongo-1.0.0/typedmongo/__init__.py` & `typedmongo-1.0.1/typedmongo/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/typedmongo/asyncio/__init__.py` & `typedmongo-1.0.1/typedmongo/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/typedmongo/asyncio/client.py` & `typedmongo-1.0.1/typedmongo/asyncio/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/typedmongo/asyncio/fields.py` & `typedmongo-1.0.1/typedmongo/asyncio/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/typedmongo/asyncio/table.py` & `typedmongo-1.0.1/typedmongo/asyncio/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,23 +51,21 @@
         if isinstance(self.keys, Field):
             keys = self.keys.field_name
         elif isinstance(self.keys, Mapping):
             keys = {field.field_name: value for field, value in self.keys.items()}
         else:
             keys = [(field.field_name, value) for field, value in self.keys]
 
-        return IndexModel(
-            keys=keys,
-            name=self.name,
-            unique=self.unique,
-            background=self.background,
-            sparse=self.sparse,
-            expireAfterSeconds=self.expireAfterSeconds,
-            partialFilterExpression=self.partialFilterExpression,
-        )
+        parameters = dataclasses.asdict(self)
+        del parameters["keys"]
+        if parameters["partialFilterExpression"] is None:
+            del parameters["partialFilterExpression"]
+        if parameters["expireAfterSeconds"] is None:
+            del parameters["expireAfterSeconds"]
+        return IndexModel(keys=keys, **parameters)
 
 
 @dataclass_transform(eq_default=False, kw_only_default=True)
 class TableMetaClass(type):
     if TYPE_CHECKING:
         __abstract__: bool
         __database__: Any
```

### Comparing `typedmongo-1.0.0/typedmongo/client.py` & `typedmongo-1.0.1/typedmongo/client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/typedmongo/expressions.py` & `typedmongo-1.0.1/typedmongo/expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/typedmongo/fields.py` & `typedmongo-1.0.1/typedmongo/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/typedmongo/sync.py` & `typedmongo-1.0.1/typedmongo/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.0/typedmongo/table.py` & `typedmongo-1.0.1/typedmongo/table.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,23 +51,21 @@
         if isinstance(self.keys, Field):
             keys = self.keys.field_name
         elif isinstance(self.keys, Mapping):
             keys = {field.field_name: value for field, value in self.keys.items()}
         else:
             keys = [(field.field_name, value) for field, value in self.keys]
 
-        return IndexModel(
-            keys=keys,
-            name=self.name,
-            unique=self.unique,
-            background=self.background,
-            sparse=self.sparse,
-            expireAfterSeconds=self.expireAfterSeconds,
-            partialFilterExpression=self.partialFilterExpression,
-        )
+        parameters = dataclasses.asdict(self)
+        del parameters["keys"]
+        if parameters["partialFilterExpression"] is None:
+            del parameters["partialFilterExpression"]
+        if parameters["expireAfterSeconds"] is None:
+            del parameters["expireAfterSeconds"]
+        return IndexModel(keys=keys, **parameters)
 
 
 @dataclass_transform(eq_default=False, kw_only_default=True)
 class TableMetaClass(type):
     if TYPE_CHECKING:
         __abstract__: bool
         __database__: Any
@@ -178,15 +176,15 @@
 
     objects = Manager()
 
     def __repr__(self) -> str:
         return "{class_name}({fields})".format(
             class_name=self.__class__.__name__,
             fields=", ".join(
-                f"{name}={self.__dict__[name]}"
+                f"{name}={repr(self.__dict__[name])}"
                 for name, _ in self.__fields__.items()
                 if name in self.__dict__
             ),
         )
 
     @staticmethod
     def __create_schema__(name: str, fields: dict[str, Field]) -> Schema:
```

