# Comparing `tmp/sqlmodel_filters-0.0.5.tar.gz` & `tmp/sqlmodel_filters-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlmodel_filters-0.0.5.tar", max compression
+gzip compressed data, was "sqlmodel_filters-0.0.6.tar", max compression
```

## Comparing `sqlmodel_filters-0.0.5.tar` & `sqlmodel_filters-0.0.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1070 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/LICENSE
--rw-r--r--   0        0        0     7693 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/README.md
--rw-r--r--   0        0        0     1022 2024-04-15 23:23:13.105450 sqlmodel_filters-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       69 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/sqlmodel_filters/__init__.py
--rw-r--r--   0        0        0     5029 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/sqlmodel_filters/builder.py
--rw-r--r--   0        0        0     5689 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/sqlmodel_filters/components.py
--rw-r--r--   0        0        0      165 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/sqlmodel_filters/exceptions.py
--rw-r--r--   0        0        0      637 2024-04-15 23:22:56.913401 sqlmodel_filters-0.0.5/sqlmodel_filters/utils.py
--rw-r--r--   0        0        0     8278 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/LICENSE
+-rw-r--r--   0        0        0     8442 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/README.md
+-rw-r--r--   0        0        0     1022 2024-04-26 00:41:05.451602 sqlmodel_filters-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       82 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/sqlmodel_filters/__init__.py
+-rw-r--r--   0        0        0     7467 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/sqlmodel_filters/builder.py
+-rw-r--r--   0        0        0     6802 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/sqlmodel_filters/components.py
+-rw-r--r--   0        0        0      165 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/sqlmodel_filters/exceptions.py
+-rw-r--r--   0        0        0      777 2024-04-26 00:40:51.787604 sqlmodel_filters-0.0.6/sqlmodel_filters/utils.py
+-rw-r--r--   0        0        0     9027 1970-01-01 00:00:00.000000 sqlmodel_filters-0.0.6/PKG-INFO
```

### Comparing `sqlmodel_filters-0.0.5/LICENSE` & `sqlmodel_filters-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlmodel_filters-0.0.5/README.md` & `sqlmodel_filters-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -206,10 +206,36 @@
 ```py
 >>> tree = parse("name:*")
 >>> statement = builder(tree, entities=func.count(Hero.id))
 >>> session.scalar(statement)
 3
 ```
 
+## Default Fields
+
+Default fields are used if you don't set a field in a query.
+
+| Query    | SQL (Where Clause)                                                    |
+| -------- | --------------------------------------------------------------------- |
+| `Spider` | `WHERE hero.name LIKE '%Spider%' OR hero.secret_name LIKE '%Spider%'` |
+
+The default fields are fields of a model by default.
+
+You can override the default by setting `default_fields`.
+
+```py
+builder = SelectBuilder(Hero, default_fields={"name": Hero.model_fields["name"]})
+```
+
+### Helper Function
+
+`q_to_select` function parses a query and builds a select statement on the fly.
+
+```py
+from sqlmodel_filters import q_to_select
+
+statement = q_to_select('name:"Spider-Boy"', Hero)
+```
+
 ## Known Limitations / Todos
 
 - Field Grouping is not supported
```

### Comparing `sqlmodel_filters-0.0.5/pyproject.toml` & `sqlmodel_filters-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqlmodel-filters"
-version = "0.0.5"
+version = "0.0.6"
 description = "A Lucene query like fliltering for SQLModel"
 authors = ["Manabu Niseki <manabu.niseki@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sqlmodel_filters-0.0.5/sqlmodel_filters/components.py` & `sqlmodel_filters-0.0.6/sqlmodel_filters/components.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+import contextlib
+from functools import cached_property
 from types import MappingProxyType
 from typing import TypeVar
 
 from luqum.tree import From, Item, Phrase, Range, Regex, To, Word
+from pydantic.fields import FieldInfo
 from sqlalchemy.orm.attributes import InstrumentedAttribute
 from sqlalchemy.sql._typing import _ColumnExpressionArgument
 from sqlmodel import SQLModel, and_
 
 from .exceptions import IllegalFieldError, IllegalFilterError
 from .utils import cast_by_annotation, dequote, deslash
 
@@ -54,52 +57,54 @@
         *,
         relationships: MappingProxyType[str, type[SQLModel]],
     ):
         self.name = name
         self.model = model
         self.relationships = relationships
 
-        self.chains = self.name.split(".")
+    @cached_property
+    def chains(self):
+        return self.name.split(".")
 
     @property
-    def is_nested(self) -> bool:
+    def is_chained(self) -> bool:
         return len(self.chains) > 1
 
-    @property
-    def _name(self) -> str:
+    @cached_property
+    def last_name(self) -> str:
         return self.chains[-1]
 
     @property
     def _model(self):
-        if not self.is_nested:
+        if not self.is_chained:
             return self.model
 
         model = self.model
         for chain in self.chains[:-2]:
             if chain not in model.__sqlmodel_relationships__:
                 raise IllegalFieldError(f"{model.__name__} does not have field:{chain}")
 
             model = self.relationships[chain]
 
-        name = self.chains[-2]
+        relationship_name = self.chains[-2]
         try:
-            return self.relationships[name]
+            return self.relationships[relationship_name]
         except KeyError as e:
-            raise IllegalFieldError(f"{model.__name__} does not have field:{name}") from e
+            raise IllegalFieldError(f"{model.__name__} does not have field:{relationship_name}") from e
 
     @property
     def field(self) -> InstrumentedAttribute:
         try:
-            return getattr(self._model, self._name)
+            return getattr(self._model, self.last_name)
         except AttributeError as e:
-            raise IllegalFieldError(f"{self._model.__name__} does not have field:{self._name}") from e
+            raise IllegalFieldError(f"{self._model.__name__} does not have field:{self.last_name}") from e
 
     @property
     def annotation(self) -> type:
-        return self._model.model_fields[self._name].annotation  # type: ignore
+        return self._model.model_fields[self.last_name].annotation  # type: ignore
 
 
 class SearchFieldNode:
     def __init__(
         self, node: Item, *, model: type[ModelType], name: str, relationships: MappingProxyType[str, type[SQLModel]]
     ):
         self.node = node
@@ -170,7 +175,31 @@
                 yield from self._from_expression(self.node)
             case To():
                 yield from self._to_expression(self.node)
             case Regex():
                 yield from self._regex_expression(self.node)
             case unknown:
                 raise IllegalFilterError(f"{unknown.__class__} is not supported yet")
+
+
+class WordNode:
+    def __init__(self, node: Word, *, model: type[ModelType], default_fields: dict[str, FieldInfo] | None = None):
+        self.node = node
+        self.model = model
+        self.default_fields = default_fields or model.model_fields
+
+    def get_field(self, name) -> InstrumentedAttribute:
+        return getattr(self.model, name)
+
+    def get_expressions(self):
+        for name, field_info in self.default_fields.items():
+            with contextlib.suppress(Exception):
+                field = self.get_field(name)
+
+                if self.node.value == "*":
+                    yield field.isnot(None)
+                else:
+                    casted = cast_by_annotation(self.node.value, field_info.annotation)
+                    if isinstance(casted, str):
+                        yield field.like(str(LikeWord(casted)))
+                    else:
+                        yield field == casted
```

### Comparing `sqlmodel_filters-0.0.5/sqlmodel_filters/utils.py` & `sqlmodel_filters-0.0.6/sqlmodel_filters/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,25 @@
+from functools import lru_cache
 from typing import Any
 
 from pydantic import BaseModel
 
 
-def cast_by_annotation(value: Any, annotation: Any) -> Any:
+@lru_cache
+def get_converter(annotation: Any):
     # TODO: find a better way in terms of performance...
-    class Wrapper(BaseModel):
+    class Converter(BaseModel):
         value: annotation
 
-    return Wrapper(value=value).value
+    return Converter
+
+
+def cast_by_annotation(value: Any, annotation: Any) -> Any:
+    klass = get_converter(annotation)
+    return klass(value=value).value
 
 
 def is_surrounded(s: Any, prefix: str | tuple[str, ...]) -> bool:
     if isinstance(s, str):
         return s[0] == s[-1] and s.startswith(prefix)
 
     return False
```

### Comparing `sqlmodel_filters-0.0.5/PKG-INFO` & `sqlmodel_filters-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlmodel-filters
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Lucene query like fliltering for SQLModel
 License: MIT
 Author: Manabu Niseki
 Author-email: manabu.niseki@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -223,11 +223,37 @@
 ```py
 >>> tree = parse("name:*")
 >>> statement = builder(tree, entities=func.count(Hero.id))
 >>> session.scalar(statement)
 3
 ```
 
+## Default Fields
+
+Default fields are used if you don't set a field in a query.
+
+| Query    | SQL (Where Clause)                                                    |
+| -------- | --------------------------------------------------------------------- |
+| `Spider` | `WHERE hero.name LIKE '%Spider%' OR hero.secret_name LIKE '%Spider%'` |
+
+The default fields are fields of a model by default.
+
+You can override the default by setting `default_fields`.
+
+```py
+builder = SelectBuilder(Hero, default_fields={"name": Hero.model_fields["name"]})
+```
+
+### Helper Function
+
+`q_to_select` function parses a query and builds a select statement on the fly.
+
+```py
+from sqlmodel_filters import q_to_select
+
+statement = q_to_select('name:"Spider-Boy"', Hero)
+```
+
 ## Known Limitations / Todos
 
 - Field Grouping is not supported
```

