# Comparing `tmp/fractal_specifications-3.1.5.tar.gz` & `tmp/fractal_specifications-3.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_specifications-3.1.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "fractal_specifications-3.1.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fractal_specifications-3.1.5.tar` & `fractal_specifications-3.1.6.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0      187 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/.coveragerc
--rw-r--r--   0        0        0      100 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/.flake8
--rw-r--r--   0        0        0      965 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/.gitignore
--rw-r--r--   0        0        0      161 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/.isort.cfg
--rw-r--r--   0        0        0     1716 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/LICENSE
--rw-r--r--   0        0        0     1436 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/Makefile
--rw-r--r--   0        0        0    14207 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/README.md
--rw-r--r--   0        0        0      780 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/align_version.py
--rw-r--r--   0        0        0      157 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/__init__.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/django/__init__.py
--rw-r--r--   0        0        0     2689 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/django/specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     3177 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/elasticsearch/specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     2391 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/google_firestore/specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2824 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/mongo/specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4024 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/pandas/specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1609 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/contrib/sqlalchemy/specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/generic/__init__.py
--rw-r--r--   0        0        0     2041 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/generic/collections.py
--rw-r--r--   0        0        0     4878 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/generic/dsl_parser.py
--rw-r--r--   0        0        0     4436 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/generic/operators.py
--rw-r--r--   0        0        0     6609 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/generic/specification.py
--rw-r--r--   0        0        0       77 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/fractal_specifications/py.typed
--rw-r--r--   0        0        0     1713 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/pyproject.toml
--rw-r--r--   0        0        0       69 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/setup.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/contrib/django/__init__.py
--rw-r--r--   0        0        0     2761 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/contrib/django/test_specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/contrib/elasticsearch/__init__.py
--rw-r--r--   0        0        0     2447 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/contrib/elasticsearch/test_specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/contrib/google_firestore/__init__.py
--rw-r--r--   0        0        0     1724 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/contrib/google_firestore/test_specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     2205 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/contrib/mongo/test_specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/contrib/pandas/__init__.py
--rw-r--r--   0        0        0     4709 2023-11-15 13:25:05.276939 fractal_specifications-3.1.5/tests/contrib/pandas/test_specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.280939 fractal_specifications-3.1.5/tests/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0     1153 2023-11-15 13:25:05.280939 fractal_specifications-3.1.5/tests/contrib/sqlalchemy/test_specifications.py
--rw-r--r--   0        0        0       52 2023-11-15 13:25:05.280939 fractal_specifications-3.1.5/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     4254 2023-11-15 13:25:05.280939 fractal_specifications-3.1.5/tests/fixtures/specifications.py
--rw-r--r--   0        0        0        0 2023-11-15 13:25:05.280939 fractal_specifications-3.1.5/tests/generic/__init__.py
--rw-r--r--   0        0        0     3730 2023-11-15 13:25:05.280939 fractal_specifications-3.1.5/tests/generic/test_collections.py
--rw-r--r--   0        0        0     3807 2023-11-15 13:25:05.280939 fractal_specifications-3.1.5/tests/generic/test_operators.py
--rw-r--r--   0        0        0     5624 2023-11-15 13:25:05.280939 fractal_specifications-3.1.5/tests/generic/test_serialization.py
--rw-r--r--   0        0        0     4466 2023-11-15 13:25:05.280939 fractal_specifications-3.1.5/tests/generic/test_specification.py
--rw-r--r--   0        0        0      705 2023-11-15 13:25:05.280939 fractal_specifications-3.1.5/tox.ini
--rw-r--r--   0        0        0    15099 1970-01-01 00:00:00.000000 fractal_specifications-3.1.5/PKG-INFO
+-rw-r--r--   0        0        0      187 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/.coveragerc
+-rw-r--r--   0        0        0      100 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/.flake8
+-rw-r--r--   0        0        0      965 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/.gitignore
+-rw-r--r--   0        0        0      161 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/.isort.cfg
+-rw-r--r--   0        0        0     1716 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/LICENSE
+-rw-r--r--   0        0        0     1436 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/Makefile
+-rw-r--r--   0        0        0    14207 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/README.md
+-rw-r--r--   0        0        0      780 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/align_version.py
+-rw-r--r--   0        0        0      157 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/django/specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     3178 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/elasticsearch/specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     2392 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/google_firestore/specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2825 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/mongo/specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4025 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/pandas/specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1610 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/contrib/sqlalchemy/specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/generic/__init__.py
+-rw-r--r--   0        0        0     2041 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/generic/collections.py
+-rw-r--r--   0        0        0     4878 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/generic/dsl_parser.py
+-rw-r--r--   0        0        0     4436 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/generic/operators.py
+-rw-r--r--   0        0        0     6764 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/generic/specification.py
+-rw-r--r--   0        0        0       77 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/fractal_specifications/py.typed
+-rw-r--r--   0        0        0     1713 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/pyproject.toml
+-rw-r--r--   0        0        0       69 2024-04-26 15:54:18.358828 fractal_specifications-3.1.6/setup.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/__init__.py
+-rw-r--r--   0        0        0       37 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/django/__init__.py
+-rw-r--r--   0        0        0     2761 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/django/test_specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/elasticsearch/__init__.py
+-rw-r--r--   0        0        0     2447 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/elasticsearch/test_specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/google_firestore/__init__.py
+-rw-r--r--   0        0        0     1724 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/google_firestore/test_specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     2205 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/mongo/test_specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/pandas/__init__.py
+-rw-r--r--   0        0        0     4709 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/pandas/test_specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0     1153 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/contrib/sqlalchemy/test_specifications.py
+-rw-r--r--   0        0        0       52 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     4254 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/fixtures/specifications.py
+-rw-r--r--   0        0        0        0 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/generic/__init__.py
+-rw-r--r--   0        0        0     3730 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/generic/test_collections.py
+-rw-r--r--   0        0        0     3807 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/generic/test_operators.py
+-rw-r--r--   0        0        0     5624 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/generic/test_serialization.py
+-rw-r--r--   0        0        0     4579 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tests/generic/test_specification.py
+-rw-r--r--   0        0        0      707 2024-04-26 15:54:18.362828 fractal_specifications-3.1.6/tox.ini
+-rw-r--r--   0        0        0    15099 1970-01-01 00:00:00.000000 fractal_specifications-3.1.6/PKG-INFO
```

### Comparing `fractal_specifications-3.1.5/.github/workflows/build.yml` & `fractal_specifications-3.1.6/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/.github/workflows/publish.yml` & `fractal_specifications-3.1.6/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/.gitignore` & `fractal_specifications-3.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/.pre-commit-config.yaml` & `fractal_specifications-3.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/LICENSE` & `fractal_specifications-3.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/Makefile` & `fractal_specifications-3.1.6/Makefile`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/README.md` & `fractal_specifications-3.1.6/README.md`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/align_version.py` & `fractal_specifications-3.1.6/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/fractal_specifications/contrib/django/specifications.py` & `fractal_specifications-3.1.6/fractal_specifications/contrib/django/specifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from fractal_specifications.generic.specification import (
     EmptySpecification,
     Specification,
 )
 
 
 class SpecificationNotMappedToDjangoOrm(Exception):
-    ...
+    pass
 
 
 class DjangoOrmSpecificationBuilder:
     @classmethod
     def build(
         cls,
         specification: Optional[Specification] = None,
```

### Comparing `fractal_specifications-3.1.5/fractal_specifications/contrib/elasticsearch/specifications.py` & `fractal_specifications-3.1.6/fractal_specifications/contrib/elasticsearch/specifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from fractal_specifications.generic.specification import (
     EmptySpecification,
     Specification,
 )
 
 
 class SpecificationNotMappedToElastic(Exception):
-    ...
+    pass
 
 
 class ElasticSpecificationBuilder:
     @staticmethod
     def build(specification: Optional[Specification] = None) -> Optional[dict]:
         if specification is None:
             return None
```

### Comparing `fractal_specifications-3.1.5/fractal_specifications/contrib/google_firestore/specifications.py` & `fractal_specifications-3.1.6/fractal_specifications/contrib/google_firestore/specifications.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from fractal_specifications.generic.specification import (
     EmptySpecification,
     Specification,
 )
 
 
 class SpecificationNotMappedToFirestore(Exception):
-    ...
+    pass
 
 
 class FirestoreSpecificationBuilder:
     @staticmethod
     def build(specification: Optional[Specification] = None) -> Optional[Collection]:
         if specification is None:
             return None
```

### Comparing `fractal_specifications-3.1.5/fractal_specifications/contrib/mongo/specifications.py` & `fractal_specifications-3.1.6/fractal_specifications/contrib/mongo/specifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from fractal_specifications.generic.specification import (
     EmptySpecification,
     Specification,
 )
 
 
 class SpecificationNotMappedToMongo(Exception):
-    ...
+    pass
 
 
 class MongoSpecificationBuilder:
     @staticmethod
     def build(specification: Optional[Specification] = None) -> Optional[Collection]:
         if specification is None:
             return None
```

### Comparing `fractal_specifications-3.1.5/fractal_specifications/contrib/pandas/specifications.py` & `fractal_specifications-3.1.6/fractal_specifications/contrib/pandas/specifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from fractal_specifications.generic.specification import (
     EmptySpecification,
     Specification,
 )
 
 
 class SpecificationNotMappedToPandas(Exception):
-    ...
+    pass
 
 
 class PandasSpecificationBuilder:
     @classmethod
     def build(
         cls,
         specification: Optional[Specification] = None,
```

### Comparing `fractal_specifications-3.1.5/fractal_specifications/contrib/sqlalchemy/specifications.py` & `fractal_specifications-3.1.6/fractal_specifications/contrib/sqlalchemy/specifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from fractal_specifications.generic.specification import (
     EmptySpecification,
     Specification,
 )
 
 
 class SpecificationNotMappedToSqlAlchemyOrm(Exception):
-    ...
+    pass
 
 
 class SqlAlchemyOrmSpecificationBuilder:
     @staticmethod
     def build(specification: Optional[Specification] = None) -> Optional[Collection]:
         if specification is None:
             return None
```

### Comparing `fractal_specifications-3.1.5/fractal_specifications/generic/collections.py` & `fractal_specifications-3.1.6/fractal_specifications/generic/collections.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/fractal_specifications/generic/dsl_parser.py` & `fractal_specifications-3.1.6/fractal_specifications/generic/dsl_parser.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/fractal_specifications/generic/operators.py` & `fractal_specifications-3.1.6/fractal_specifications/generic/operators.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/fractal_specifications/generic/specification.py` & `fractal_specifications-3.1.6/fractal_specifications/generic/specification.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,26 +28,28 @@
             "!": operators.NotSpecification,
             "&": collections.AndSpecification,
             "|": collections.OrSpecification,
         },
     }
 
 
-def _parse_specification_item(field_op: str, value: Any) -> Optional[Specification]:
+def _parse_specification_item(
+    field_op: str, value: Any, lookup_separator: str
+) -> Optional[Specification]:
     parts = field_op.split("__")
-    field = ".".join(parts[:-1])
+    field = lookup_separator.join(parts[:-1])
     op = parts[-1]
     if spec := all_specifications().get(op, None):
         return spec(field, value)
-    return all_specifications()["=="](".".join(parts), value)
+    return all_specifications()["=="](lookup_separator.join(parts), value)
 
 
-def parse_specification(**kwargs) -> Iterator[Specification]:
+def parse_specification(lookup_separator: str, **kwargs) -> Iterator[Specification]:
     for field_op, value in kwargs.items():
-        if spec := _parse_specification_item(field_op, value):
+        if spec := _parse_specification_item(field_op, value, lookup_separator):
             yield spec
 
 
 SpecificationSubType = TypeVar("SpecificationSubType", bound="Specification")
 
 
 class Specification(ABC):
@@ -88,16 +90,16 @@
     @staticmethod
     def Not(specification: "Specification") -> "Specification":
         from fractal_specifications.generic.operators import NotSpecification
 
         return NotSpecification(specification)
 
     @staticmethod
-    def parse(**kwargs):
-        specs = list(parse_specification(**kwargs))
+    def parse(_lookup_separator=".", **kwargs):
+        specs = list(parse_specification(lookup_separator=_lookup_separator, **kwargs))
         if len(specs) > 1:
             from fractal_specifications.generic.collections import AndSpecification
 
             return AndSpecification(specs)
         elif len(specs) == 1:
             return specs[0]
         return None
```

### Comparing `fractal_specifications-3.1.5/pyproject.toml` & `fractal_specifications-3.1.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-specifications"
-version = "3.1.5"
+version = "3.1.6"
 description = "Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [tool.poetry.dependencies]
 lark = "*"
 
 [build-system]
```

### Comparing `fractal_specifications-3.1.5/tests/contrib/django/test_specifications.py` & `fractal_specifications-3.1.6/tests/contrib/django/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/tests/contrib/elasticsearch/test_specifications.py` & `fractal_specifications-3.1.6/tests/contrib/elasticsearch/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/tests/contrib/google_firestore/test_specifications.py` & `fractal_specifications-3.1.6/tests/contrib/google_firestore/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/tests/contrib/mongo/test_specifications.py` & `fractal_specifications-3.1.6/tests/contrib/mongo/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/tests/contrib/pandas/test_specifications.py` & `fractal_specifications-3.1.6/tests/contrib/pandas/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/tests/contrib/sqlalchemy/test_specifications.py` & `fractal_specifications-3.1.6/tests/contrib/sqlalchemy/test_specifications.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/tests/fixtures/specifications.py` & `fractal_specifications-3.1.6/tests/fixtures/specifications.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/tests/generic/test_collections.py` & `fractal_specifications-3.1.6/tests/generic/test_collections.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/tests/generic/test_operators.py` & `fractal_specifications-3.1.6/tests/generic/test_operators.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/tests/generic/test_serialization.py` & `fractal_specifications-3.1.6/tests/generic/test_serialization.py`

 * *Files identical despite different names*

### Comparing `fractal_specifications-3.1.5/tests/generic/test_specification.py` & `fractal_specifications-3.1.6/tests/generic/test_specification.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,17 @@
 )
 
 
 def test_parse():
     assert Specification.parse(id=1) == EqualsSpecification("id", 1)
     assert Specification.parse(id_x=1) == EqualsSpecification("id_x", 1)
     assert Specification.parse(id__x=1) == EqualsSpecification("id.x", 1)
+    assert Specification.parse(id__x=1, _lookup_separator="__") == EqualsSpecification(
+        "id__x", 1
+    )
     assert Specification.parse(id__eq=1) == EqualsSpecification("id", 1)
     assert Specification.parse(obj__id__eq=1) == EqualsSpecification("obj.id", 1)
     assert Specification.parse(id__in=[1]) == InSpecification("id", [1])
     assert Specification.parse(id__contains="a") == ContainsSpecification("id", "a")
     assert Specification.parse(name__matches=r"^.*$") == RegexStringMatchSpecification(
         "name", r"^.*$"
     )
```

### Comparing `fractal_specifications-3.1.5/tox.ini` & `fractal_specifications-3.1.6/tox.ini`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     flake8
     flit
     isort
     lark
     mccabe
     mypy
     pylint
-    pytest
+    pytest<7
     pytest-cov
     pytest-asyncio
     pytest-lazy-fixture
     tox
     tox-gh-actions
     pre-commit
     autoflake
```

### Comparing `fractal_specifications-3.1.5/PKG-INFO` & `fractal_specifications-3.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-specifications
-Version: 3.1.5
+Version: 3.1.6
 Summary: Fractal Specifications is an implementation of the specification pattern for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-specifications
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
```

