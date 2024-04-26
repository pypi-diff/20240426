# Comparing `tmp/typedmongo-1.0.2.tar.gz` & `tmp/typedmongo-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typedmongo-1.0.2.tar", last modified: Fri Apr 26 02:45:24 2024, max compression
+gzip compressed data, was "typedmongo-1.0.3.tar", last modified: Fri Apr 26 06:44:18 2024, max compression
```

## Comparing `typedmongo-1.0.2.tar` & `typedmongo-1.0.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-26 02:45:12.707974 typedmongo-1.0.2/LICENSE
--rw-r--r--   0        0        0      108 2024-04-26 02:45:12.707974 typedmongo-1.0.2/README.md
--rw-r--r--   0        0        0     1441 2024-04-26 02:45:24.783982 typedmongo-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-26 02:45:12.707974 typedmongo-1.0.2/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-04-26 02:45:12.707974 typedmongo-1.0.2/tests/asyncio/__init__.py
--rw-r--r--   0        0        0     5783 2024-04-26 02:45:12.707974 typedmongo-1.0.2/tests/asyncio/test_client.py
--rw-r--r--   0        0        0     2620 2024-04-26 02:45:12.707974 typedmongo-1.0.2/tests/asyncio/test_table.py
--rw-r--r--   0        0        0     1218 2024-04-26 02:45:12.707974 typedmongo-1.0.2/tests/sync.py
--rw-r--r--   0        0        0     5549 2024-04-26 02:45:12.707974 typedmongo-1.0.2/tests/test_client.py
--rw-r--r--   0        0        0     2930 2024-04-26 02:45:12.707974 typedmongo-1.0.2/tests/test_expressions.py
--rw-r--r--   0        0        0      582 2024-04-26 02:45:12.707974 typedmongo-1.0.2/tests/test_marshamallow.py
--rw-r--r--   0        0        0     2612 2024-04-26 02:45:12.707974 typedmongo-1.0.2/tests/test_table.py
--rw-r--r--   0        0        0      749 2024-04-26 02:45:12.707974 typedmongo-1.0.2/typedmongo/__init__.py
--rw-r--r--   0        0        0      749 2024-04-26 02:45:12.707974 typedmongo-1.0.2/typedmongo/asyncio/__init__.py
--rw-r--r--   0        0        0    11778 2024-04-26 02:45:12.707974 typedmongo-1.0.2/typedmongo/asyncio/client.py
--rw-r--r--   0        0        0     8660 2024-04-26 02:45:12.707974 typedmongo-1.0.2/typedmongo/asyncio/fields.py
--rw-r--r--   0        0        0     6982 2024-04-26 02:45:12.711974 typedmongo-1.0.2/typedmongo/asyncio/table.py
--rw-r--r--   0        0        0    11560 2024-04-26 02:45:12.711974 typedmongo-1.0.2/typedmongo/client.py
--rw-r--r--   0        0        0      163 2024-04-26 02:45:12.711974 typedmongo-1.0.2/typedmongo/exceptions.py
--rw-r--r--   0        0        0     5452 2024-04-26 02:45:12.711974 typedmongo-1.0.2/typedmongo/expressions.py
--rw-r--r--   0        0        0     8660 2024-04-26 02:45:12.711974 typedmongo-1.0.2/typedmongo/fields.py
--rw-r--r--   0        0        0      351 2024-04-26 02:45:12.711974 typedmongo-1.0.2/typedmongo/marshamallow.py
--rw-r--r--   0        0        0     1325 2024-04-26 02:45:12.711974 typedmongo-1.0.2/typedmongo/sync.py
--rw-r--r--   0        0        0     6982 2024-04-26 02:45:12.711974 typedmongo-1.0.2/typedmongo/table.py
--rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-26 06:44:05.701338 typedmongo-1.0.3/LICENSE
+-rw-r--r--   0        0        0      108 2024-04-26 06:44:05.701338 typedmongo-1.0.3/README.md
+-rw-r--r--   0        0        0     1441 2024-04-26 06:44:18.857402 typedmongo-1.0.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-26 06:44:05.701338 typedmongo-1.0.3/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 06:44:05.701338 typedmongo-1.0.3/tests/asyncio/__init__.py
+-rw-r--r--   0        0        0     5789 2024-04-26 06:44:05.701338 typedmongo-1.0.3/tests/asyncio/test_client.py
+-rw-r--r--   0        0        0     2620 2024-04-26 06:44:05.701338 typedmongo-1.0.3/tests/asyncio/test_table.py
+-rw-r--r--   0        0        0     1218 2024-04-26 06:44:05.705338 typedmongo-1.0.3/tests/sync.py
+-rw-r--r--   0        0        0     5549 2024-04-26 06:44:05.705338 typedmongo-1.0.3/tests/test_client.py
+-rw-r--r--   0        0        0     2930 2024-04-26 06:44:05.705338 typedmongo-1.0.3/tests/test_expressions.py
+-rw-r--r--   0        0        0      582 2024-04-26 06:44:05.705338 typedmongo-1.0.3/tests/test_marshamallow.py
+-rw-r--r--   0        0        0     2612 2024-04-26 06:44:05.705338 typedmongo-1.0.3/tests/test_table.py
+-rw-r--r--   0        0        0      749 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/__init__.py
+-rw-r--r--   0        0        0      749 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/asyncio/__init__.py
+-rw-r--r--   0        0        0    11769 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/asyncio/client.py
+-rw-r--r--   0        0        0     8660 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/asyncio/fields.py
+-rw-r--r--   0        0        0     6982 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/asyncio/table.py
+-rw-r--r--   0        0        0    11551 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/client.py
+-rw-r--r--   0        0        0      163 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/exceptions.py
+-rw-r--r--   0        0        0     5452 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/expressions.py
+-rw-r--r--   0        0        0     8660 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/fields.py
+-rw-r--r--   0        0        0      351 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/marshamallow.py
+-rw-r--r--   0        0        0     1325 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/sync.py
+-rw-r--r--   0        0        0     6982 2024-04-26 06:44:05.705338 typedmongo-1.0.3/typedmongo/table.py
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 typedmongo-1.0.3/PKG-INFO
```

### Comparing `typedmongo-1.0.2/LICENSE` & `typedmongo-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/pyproject.toml` & `typedmongo-1.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "typedmongo"
-version = "1.0.2"
+version = "1.0.3"
 description = "A production-ready modern Python MongoDB ODM"
 authors = [
     { name = "abersheeran", email = "me@abersheeran.com" },
 ]
 dependencies = [
     "pymongo>=4.6.3",
     "motor>=3.4.0",
```

### Comparing `typedmongo-1.0.2/tests/asyncio/test_client.py` & `typedmongo-1.0.3/tests/asyncio/test_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -194,9 +194,9 @@
     "projection",
     [
         [User.name],
         {User.name: True, User._id: False},
     ],
 )
 async def test_projection(documents_id, projection):
-    user = User.objects.find_one(User.age == 18, projection=projection)
+    user = await User.objects.find_one(User.age == 18, projection=projection)
     assert user is not None
```

### Comparing `typedmongo-1.0.2/tests/asyncio/test_table.py` & `typedmongo-1.0.3/tests/asyncio/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/tests/sync.py` & `typedmongo-1.0.3/tests/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/tests/test_client.py` & `typedmongo-1.0.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/tests/test_expressions.py` & `typedmongo-1.0.3/tests/test_expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/tests/test_marshamallow.py` & `typedmongo-1.0.3/tests/test_marshamallow.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/tests/test_table.py` & `typedmongo-1.0.3/tests/test_table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/typedmongo/__init__.py` & `typedmongo-1.0.3/typedmongo/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/typedmongo/asyncio/__init__.py` & `typedmongo-1.0.3/typedmongo/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/typedmongo/asyncio/client.py` & `typedmongo-1.0.3/typedmongo/asyncio/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     from pymongo.results import BulkWriteResult as MongoBlukWriteResult
     from pymongo.results import DeleteResult as MongoDeleteResult
     from pymongo.results import UpdateResult as MongoUpdateResult
 
     from .table import Table
 
 from typedmongo.expressions import Expression, OrderBy, compile_expression
-from typedmongo.fields import Field
+
+from .fields import Field
 
 DocumentId: TypeAlias = Any
 T = TypeVar("T", bound="Table")
 
 
 class DecimalCodec(TypeCodec):
     python_type = decimal.Decimal  # type: ignore
```

### Comparing `typedmongo-1.0.2/typedmongo/asyncio/fields.py` & `typedmongo-1.0.3/typedmongo/asyncio/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/typedmongo/asyncio/table.py` & `typedmongo-1.0.3/typedmongo/asyncio/table.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/typedmongo/client.py` & `typedmongo-1.0.3/typedmongo/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,16 @@
     from pymongo.results import BulkWriteResult as MongoBlukWriteResult
     from pymongo.results import DeleteResult as MongoDeleteResult
     from pymongo.results import UpdateResult as MongoUpdateResult
 
     from .table import Table
 
 from typedmongo.expressions import Expression, OrderBy, compile_expression
-from typedmongo.fields import Field
+
+from .fields import Field
 
 DocumentId: TypeAlias = Any
 T = TypeVar("T", bound="Table")
 
 
 class DecimalCodec(TypeCodec):
     python_type = decimal.Decimal  # type: ignore
```

### Comparing `typedmongo-1.0.2/typedmongo/expressions.py` & `typedmongo-1.0.3/typedmongo/expressions.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/typedmongo/fields.py` & `typedmongo-1.0.3/typedmongo/fields.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/typedmongo/sync.py` & `typedmongo-1.0.3/typedmongo/sync.py`

 * *Files identical despite different names*

### Comparing `typedmongo-1.0.2/typedmongo/table.py` & `typedmongo-1.0.3/typedmongo/table.py`

 * *Files identical despite different names*

