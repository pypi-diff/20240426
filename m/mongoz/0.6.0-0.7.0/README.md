# Comparing `tmp/mongoz-0.6.0.tar.gz` & `tmp/mongoz-0.7.0.tar.gz`

## Comparing `mongoz-0.6.0.tar` & `mongoz-0.7.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
--rw-r--r--   0        0        0     1494 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/__init__.py
--rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/exceptions.py
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/py.typed
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/types.py
--rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/conf/__init__.py
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/conf/functional.py
--rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/conf/global_settings.py
--rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/conf/module_import.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/__init__.py
--rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/connection/__init__.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/connection/collections.py
--rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/connection/database.py
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/connection/registry.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/__init__.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/datastructures.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/documents/__init__.py
--rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/documents/_internal.py
--rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/documents/base.py
--rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/documents/document.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/documents/document_proxy.py
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/documents/document_row.py
--rw-r--r--   0        0        0    16216 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/documents/metaclasses.py
--rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/fields/__init__.py
--rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/fields/base.py
--rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/fields/core.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/querysets/__init__.py
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/querysets/base.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/querysets/expressions.py
--rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/querysets/operators.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/querysets/core/constants.py
--rw-r--r--   0        0        0    21681 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/querysets/core/manager.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/querysets/core/protocols.py
--rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/db/querysets/core/queryset.py
--rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/signals/__init__.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/signals/handlers.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/signals/signal.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/utils/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/utils/documents.py
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/utils/functional.py
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/core/utils/sync.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/protocols/__init__.py
--rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/protocols/queryset.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/utils/__init__.py
--rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/utils/enums.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/utils/inspect.py
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mongoz-0.6.0/mongoz/utils/mixins.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mongoz-0.6.0/.gitignore
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mongoz-0.6.0/LICENSE
--rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 mongoz-0.6.0/README.md
--rw-r--r--   0        0        0     3936 2020-02-02 00:00:00.000000 mongoz-0.6.0/pyproject.toml
--rw-r--r--   0        0        0    10208 2020-02-02 00:00:00.000000 mongoz-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/__init__.py
+-rw-r--r--   0        0        0      960 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/exceptions.py
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/py.typed
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/types.py
+-rw-r--r--   0        0        0     1775 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/conf/__init__.py
+-rw-r--r--   0        0        0     4975 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/conf/functional.py
+-rw-r--r--   0        0        0     1669 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/conf/global_settings.py
+-rw-r--r--   0        0        0      727 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/conf/module_import.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/__init__.py
+-rw-r--r--   0        0        0      136 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/connection/__init__.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/connection/collections.py
+-rw-r--r--   0        0        0     1166 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/connection/database.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/connection/registry.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/__init__.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/datastructures.py
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/__init__.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/_internal.py
+-rw-r--r--   0        0        0     5957 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/base.py
+-rw-r--r--   0        0        0     6838 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/document.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/document_proxy.py
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/document_row.py
+-rw-r--r--   0        0        0      927 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/managers.py
+-rw-r--r--   0        0        0    16421 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/documents/metaclasses.py
+-rw-r--r--   0        0        0      525 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/fields/__init__.py
+-rw-r--r--   0        0        0     6531 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/fields/base.py
+-rw-r--r--   0        0        0    11761 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/fields/core.py
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/__init__.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/base.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/expressions.py
+-rw-r--r--   0        0        0     5190 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/operators.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/core/constants.py
+-rw-r--r--   0        0        0    21681 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/core/manager.py
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/core/protocols.py
+-rw-r--r--   0        0        0    12693 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/db/querysets/core/queryset.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/signals/__init__.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/signals/handlers.py
+-rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/signals/signal.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/utils/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/utils/documents.py
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/utils/functional.py
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/core/utils/sync.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/protocols/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/protocols/queryset.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/utils/__init__.py
+-rw-r--r--   0        0        0      681 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/utils/enums.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/utils/inspect.py
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 mongoz-0.7.0/mongoz/utils/mixins.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 mongoz-0.7.0/.gitignore
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 mongoz-0.7.0/LICENSE
+-rw-r--r--   0        0        0     7029 2020-02-02 00:00:00.000000 mongoz-0.7.0/README.md
+-rw-r--r--   0        0        0     3761 2020-02-02 00:00:00.000000 mongoz-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 mongoz-0.7.0/PKG-INFO
```

### Comparing `mongoz-0.6.0/mongoz/__init__.py` & `mongoz-0.7.0/mongoz/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
-__version__ = "0.6.0"
+__version__ = "0.7.0"
 
 from .conf import settings
 from .conf.global_settings import MongozSettings
 from .core.connection.database import Database
 from .core.connection.registry import Registry
 from .core.db import fields
 from .core.db.datastructures import Index, IndexType, Order
 from .core.db.documents import Document, EmbeddedDocument
+from .core.db.documents.managers import QuerySetManager
 from .core.db.fields import (
     UUID,
     Array,
     ArrayList,
     Binary,
     Boolean,
     Date,
@@ -57,14 +58,15 @@
     "MongozSettings",
     "MultipleDocumentsReturned",
     "Object",
     "ObjectId",
     "Order",
     "Q",
     "QuerySet",
+    "QuerySetManager",
     "Registry",
     "Signal",
     "SortExpression",
     "String",
     "Time",
     "UUID",
     "settings",
```

### Comparing `mongoz-0.6.0/mongoz/exceptions.py` & `mongoz-0.7.0/mongoz/exceptions.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/conf/__init__.py` & `mongoz-0.7.0/mongoz/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/conf/functional.py` & `mongoz-0.7.0/mongoz/conf/functional.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     __lt__ = new_method_proxy(operator.lt)
     __gt__ = new_method_proxy(operator.gt)
     __ne__ = new_method_proxy(operator.ne)
     __hash__ = new_method_proxy(hash)
     __getitem__ = new_method_proxy(operator.getitem)
     __setitem__ = new_method_proxy(operator.setitem)
     __delitem__ = new_method_proxy(operator.delitem)
-    __iter__ = new_method_proxy(iter)
+    __iter__ = new_method_proxy(iter)  # type: ignore
     __len__ = new_method_proxy(len)
     __contains__ = new_method_proxy(operator.contains)
 
 
 def unpickle_lazyobject(wrapped: Any) -> Any:  # pragma: no cover
     """
     Used to unpickle lazy objects. Just return its argument, which will be the
```

### Comparing `mongoz-0.6.0/mongoz/conf/global_settings.py` & `mongoz-0.7.0/mongoz/conf/global_settings.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/conf/module_import.py` & `mongoz-0.7.0/mongoz/conf/module_import.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/connection/database.py` & `mongoz-0.7.0/mongoz/core/connection/database.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/connection/registry.py` & `mongoz-0.7.0/mongoz/core/connection/registry.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,23 +27,23 @@
 
     @property
     def address(self) -> Tuple[str, int]:
         return cast(Tuple[str, int], self._client.address)
 
     @property
     def host(self) -> str:
-        return cast(str, self._client.HOST)
+        return self._client.HOST
 
     @property
     def port(self) -> str:
         return cast(str, self._client.PORT)
 
     @property
     def driver(self) -> AsyncIOMotorDatabase:
-        return cast(AsyncIOMotorDatabase, self._client.driver)
+        return self._client.driver
 
     async def drop_database(self, database: Union[str, Database]) -> None:
         """
         Drops an existing mongo db database/
         """
         if not isinstance(database, Database):
             await self._client.drop_database(database)
```

### Comparing `mongoz-0.6.0/mongoz/core/db/datastructures.py` & `mongoz-0.7.0/mongoz/core/db/datastructures.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/db/documents/base.py` & `mongoz-0.7.0/mongoz/core/db/documents/base.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/db/documents/document.py` & `mongoz-0.7.0/mongoz/core/db/documents/document.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/db/documents/document_proxy.py` & `mongoz-0.7.0/mongoz/core/db/documents/document_proxy.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/db/documents/document_row.py` & `mongoz-0.7.0/mongoz/core/db/documents/document_row.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/db/documents/metaclasses.py` & `mongoz-0.7.0/mongoz/core/db/documents/metaclasses.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
                 break
             raise ImproperlyConfigured(
                 "database must be a string name or an instance of mongoz.Database."
             )
 
     if not found_database:
         raise ImproperlyConfigured(
-            "Database for the table not found in the Meta class or any of the superclasses. You must set the database in the Meta."
+            "'database' for the table not found in the Meta class or any of the superclasses. You must set the database in the Meta."
         )
     return found_database
 
 
 def _register_document_signals(model_class: Type["Document"]) -> None:
     """
     Registers the signals in the model's Broadcaster and sets the defaults.
@@ -231,16 +231,16 @@
             __search_for_fields(base, inherited_fields)
 
         if inherited_fields:
             # Making sure the inherited fields are before the new defined.
             attrs = {**inherited_fields, **attrs}
 
         for key, value in attrs.items():
-            if isinstance(value, BaseField):
-                if getattr(meta_class, "abstract", None) is None:
+            if isinstance(value, (BaseField)):
+                if getattr(meta_class, "abstract", None):
                     value = copy.copy(value)
                 fields[key] = value
 
         for slot in fields:
             attrs.pop(slot, None)
 
         attrs["meta"] = meta = MetaInfo(meta_class)
@@ -257,18 +257,24 @@
         parents = [parent for parent in bases if isinstance(parent, BaseModelMeta)]
         if not parents:
             return model_class(cls, name, bases, attrs)
 
         meta.parents = parents
         new_class = cast("Type[Document]", model_class(cls, name, bases, attrs))
 
+        # Update the model_fields are updated to the latest
+        new_class.model_fields.update(model_fields)
+
         # Abstract classes do not allow multiple managers. This make sure it is enforced.
-        managers = [k for k, v in attrs.items() if isinstance(v, Manager)]
-        if len(managers) > 1:
-            raise ImproperlyConfigured("Multiple managers are not allowed.")
+        if meta.abstract:
+            managers = [k for k, v in attrs.items() if isinstance(v, Manager)]
+            if len(managers) > 1:
+                raise ImproperlyConfigured(
+                    "Multiple managers are not allowed in abstract classes."
+                )
 
         if "id" in new_class.model_fields:
             new_class.model_fields["id"].default = None
 
         # Handle the registry of models
         if getattr(meta, "registry", None) is None:
             if hasattr(new_class, "__db_document__") and new_class.__db_document__:
```

### Comparing `mongoz-0.6.0/mongoz/core/db/fields/__init__.py` & `mongoz-0.7.0/mongoz/core/db/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/db/fields/base.py` & `mongoz-0.7.0/mongoz/core/db/fields/base.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/db/fields/core.py` & `mongoz-0.7.0/mongoz/core/db/fields/core.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/db/querysets/expressions.py` & `mongoz-0.7.0/mongoz/core/db/querysets/expressions.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/db/querysets/operators.py` & `mongoz-0.7.0/mongoz/core/db/querysets/operators.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/db/querysets/core/manager.py` & `mongoz-0.7.0/mongoz/core/db/querysets/core/manager.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/db/querysets/core/queryset.py` & `mongoz-0.7.0/mongoz/core/db/querysets/core/queryset.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/signals/handlers.py` & `mongoz-0.7.0/mongoz/core/signals/handlers.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/signals/signal.py` & `mongoz-0.7.0/mongoz/core/signals/signal.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/utils/documents.py` & `mongoz-0.7.0/mongoz/core/utils/documents.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/core/utils/functional.py` & `mongoz-0.7.0/mongoz/core/utils/functional.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/protocols/queryset.py` & `mongoz-0.7.0/mongoz/protocols/queryset.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/mongoz/utils/enums.py` & `mongoz-0.7.0/mongoz/utils/enums.py`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/LICENSE` & `mongoz-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/README.md` & `mongoz-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `mongoz-0.6.0/pyproject.toml` & `mongoz-0.7.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -54,26 +54,31 @@
 Source = "https://github.com/tarsil/mongoz"
 
 [project.optional-dependencies]
 test = [
     "a2wsgi>1.10.0,<2.0.0",
     "autoflake>=2.0.2,<3.0.0",
     "black==24.1.1,<25.0",
-    "esmerald>=2.0.6",
+    "esmerald>=3.0.0",
     "httpx>=0.25.0,<0.30.0",
     "isort>=5.12.0,<6.0.0",
-    "mypy==1.5.1",
+    "mypy==1.9.0",
     "pytest>=7.2.2,<9.0.0",
     "pytest-asyncio>=0.21.1,<1.0.0",
     "pytest-cov>=4.0.0,<5.0.0",
     "requests>=2.28.2",
     "ruff>=0.0.256,<1.0.0",
 ]
 
-dev = ["anyio>=4.0.0,<5", "ipdb>=0.13.13,<1.0.0", "pre-commit>=3.3.1,<4.0.0"]
+dev = [
+    "anyio>=4.0.0,<5",
+    "ipdb>=0.13.13,<1.0.0",
+    "pdbpp",
+    "pre-commit>=3.3.1,<4.0.0",
+]
 
 doc = [
     "mkautodoc>=0.2.0,<0.3.0",
     "mkdocs>=1.4.2,<2.0.0",
     "mkdocs-material==9.1.5",
     "mdx-include>=1.4.1,<2.0.0",
     "mkdocs-markdownextradata-plugin>=0.1.7,<0.3.0",
@@ -96,31 +101,21 @@
 strict = true
 disallow_untyped_decorators = true
 disallow_any_generics = false
 implicit_reexport = false
 no_implicit_optional = false
 show_error_codes = true
 disallow_incomplete_defs = true
-disable_error_code = "attr-defined,arg-type,override,misc,valid-type,call-overload"
+disable_error_code = "attr-defined,arg-type,override,misc,valid-type,call-overload,no-any-return"
 warn_unused_ignores = true
 warn_redundant_casts = true
 
-[tool.ruff]
-select = [
-    "E", # pycodestyle errors
-    "W", # pycodestyle warnings
-    "F", # pyflakes
-    "C", # flake8-comprehensions
-    "B", # flake8-bugbear
-]
-ignore = [
-    "E501", # line too long, handled by black
-    "B008", # do not perform function calls in argument defaults
-    "C901", # too complex
-]
+[tool.ruff.lint]
+select = ["E", "W", "F", "C", "B", "I"]
+ignore = ["E501", "B008", "C901", "B026"]
 
 exclude = ["docs_src/"]
 
 [tool.coverage.run]
 parallel = true
 context = '${CONTEXT}'
 source = ["tests", "mongoz"]
```

### Comparing `mongoz-0.6.0/PKG-INFO` & `mongoz-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: mongoz
-Version: 0.6.0
+Version: 0.7.0
 Summary: ODM with pydantic made it simple
 Project-URL: Homepage, https://github.com/tarsil/mongoz
 Project-URL: Documentation, https://mongoz.tarsild.io
 Project-URL: Changelog, https://mongoz.tarsild.io/release-notes/
 Project-URL: Funding, https://github.com/sponsors/tarsil
 Project-URL: Source, https://github.com/tarsil/mongoz
 Author-email: Tiago Silva <tiago.arasivla@gmail.com>
@@ -40,31 +40,32 @@
 Requires-Dist: dymmond-settings>=1.0.4
 Requires-Dist: motor>=3.3.1
 Requires-Dist: orjson>=3.9.5
 Requires-Dist: pydantic<3.0.0,>=2.5.3
 Provides-Extra: dev
 Requires-Dist: anyio<5,>=4.0.0; extra == 'dev'
 Requires-Dist: ipdb<1.0.0,>=0.13.13; extra == 'dev'
+Requires-Dist: pdbpp; extra == 'dev'
 Requires-Dist: pre-commit<4.0.0,>=3.3.1; extra == 'dev'
 Provides-Extra: doc
 Requires-Dist: mdx-include<2.0.0,>=1.4.1; extra == 'doc'
 Requires-Dist: mkautodoc<0.3.0,>=0.2.0; extra == 'doc'
 Requires-Dist: mkdocs-markdownextradata-plugin<0.3.0,>=0.1.7; extra == 'doc'
 Requires-Dist: mkdocs-material==9.1.5; extra == 'doc'
 Requires-Dist: mkdocs<2.0.0,>=1.4.2; extra == 'doc'
 Requires-Dist: mkdocstrings<0.21.0,>=0.19.0; extra == 'doc'
 Requires-Dist: pyyaml<7.0.0,>=5.3.1; extra == 'doc'
 Provides-Extra: test
 Requires-Dist: a2wsgi<2.0.0,>1.10.0; extra == 'test'
 Requires-Dist: autoflake<3.0.0,>=2.0.2; extra == 'test'
 Requires-Dist: black<25.0,==24.1.1; extra == 'test'
-Requires-Dist: esmerald>=2.0.6; extra == 'test'
+Requires-Dist: esmerald>=3.0.0; extra == 'test'
 Requires-Dist: httpx<0.30.0,>=0.25.0; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.12.0; extra == 'test'
-Requires-Dist: mypy==1.5.1; extra == 'test'
+Requires-Dist: mypy==1.9.0; extra == 'test'
 Requires-Dist: pytest-asyncio<1.0.0,>=0.21.1; extra == 'test'
 Requires-Dist: pytest-cov<5.0.0,>=4.0.0; extra == 'test'
 Requires-Dist: pytest<9.0.0,>=7.2.2; extra == 'test'
 Requires-Dist: requests>=2.28.2; extra == 'test'
 Requires-Dist: ruff<1.0.0,>=0.0.256; extra == 'test'
 Description-Content-Type: text/markdown
```

